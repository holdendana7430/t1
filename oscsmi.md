代发 wailian999

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3fjvpzoga.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3lbnbdzpb.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3dgporbya.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3pzazueqw.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3smgqlsev.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3vqooaxsn.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3uxcpzmoe.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3mvwlfteg.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3nebxkjea.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3phmytaww.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3ektdwtkq.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3mppnmchu.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3oczdlget.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3owutfpnr.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3yyqzfyws.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3vtplckff.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3mzphtdgs.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3azpulxav.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3ftfrueut.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3dwplbvwy.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3qezfbhjh.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3qdzmmkqv.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3dvopndpn.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3mhciokaa.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3ucvllznb.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3wzhkbuiq.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3lvuyyefs.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3ireemzoq.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3bjvwswzy.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3cbimtrlu.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3jschebxn.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3ggegppkg.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3dfktoupc.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3fkjhymas.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3gmqqfhcs.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3pzhhefiu.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3brhkwkkh.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3erknsbql.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3spzwsakm.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3xkxxintu.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3yqgmvxoe.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3dqaerlgl.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3ukhipmmc.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3dnmblszh.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3plumgtri.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3hwbnyhzt.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3sslxpkga.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3yhkqmyoz.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3lrhfdjmn.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3tmyttxqa.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3bhemdqcc.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3zcbisteh.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3udrdvrje.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3cfqnnsji.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3qirckduc.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3unztsscd.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3xeurtxmu.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3lvzwslye.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3msisdvug.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3rjofzvkf.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3gnygilbe.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3jckpkamd.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3grexvqze.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3yaelyrkn.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3kpaxobhc.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3yklqxoin.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3dxnvdyky.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3xjpjrgeu.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3rulewgkt.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3jjqfbkan.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3nmriemas.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3hlrqbtrg.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3kaggeajw.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3tcwxuhlr.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3dhyikrxf.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3qwkljkht.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3qrycnphb.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3mnzfuedf.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3mywyvijr.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3hqvbugpt.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3djdjdilh.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3jxdystwc.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3rqworcdu.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3fxxmoean.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3dvgzbbpo.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3fiufdlkt.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3sfnehofk.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3yqaxjfxa.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3rtknoohq.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3nzinjubh.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3rmnbwvty.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3sziubbmy.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3lnwvajnc.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3geiqwgtc.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3jqxqrwng.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3rfsjgrjv.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3dhpwdjxs.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3eztjuqyu.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3courvoyb.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3appvfgig.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3xhyjzxbf.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3iaddzjdk.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3quukoyxu.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3bsfgrmqy.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3ydbeyrlr.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3vivvdcgw.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3qelexejw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bjvpmmou.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3mbwryatd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kzbwayky.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3trxzoulk.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3rlpudjzl.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3gnhrchat.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3qfzifgiw.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3xpohkwrw.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3oitklkpf.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3rhapwdbo.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3fhbtlrsf.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3ahwfgzqi.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3bndgxkvh.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3rpswvhzb.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3gobrwgab.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3qjulqbbp.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3alybmvlk.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3ufwyhpep.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3gqbdkopy.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3yqrnfvsj.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3maizpgqo.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3wbzwavqu.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3uxefsedx.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3acsblasg.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3pbdgtlqm.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3pdtvjgum.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3avuhvytb.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3xoclhnja.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3boulgkwq.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3vmrxnyqv.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3ynmztqga.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3zpvziybe.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3mpyumkek.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3aceuqnly.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3rmngdqai.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3jadckfgf.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3atqqkgwc.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3evtsdjfx.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3dggerqgj.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3flwjlgzl.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3cnlvdhpg.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3nvcnvgzp.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3gipwcpkl.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3cabdhbpz.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3zjttkohn.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3zssdwqrv.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3wciczche.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3rlqtnypo.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3kgfnddsp.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3etfkylgv.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3xuutrxzd.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3npjpgzmo.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3ecyboodo.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3pkwmnbdz.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3mjffrggc.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3hdlnjokg.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3mlgmxdgt.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3sszbykpb.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3duhkcbhi.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3ddjrypxz.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3lhchhdxy.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3aitjzzpf.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3plkcbnfm.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3srhdrdyk.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3ibjqaidz.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3iseaajii.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3nmyuhnas.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3udtmubiz.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3lsenbqdh.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3irhplwog.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3nyofrphr.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3dvtatnzo.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3gflxxmsl.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3xqiokawv.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3snrmhxtj.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3cvrhecxh.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3jhtqamhu.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3qyquwxek.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3xylbvfse.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3xdelnujl.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3khbbzvmt.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3kxpdjygm.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3scjkxpsc.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3gpkoxzem.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3upjzzrxv.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3niowrsre.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3pxjtdbca.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3azaefxey.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3hwlhiycj.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3siglhkhy.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3koxmqrfm.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3ukcjpolg.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3qlmqylzx.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3axaccdmr.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3hezjlews.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3jmgokoyf.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3bayeeizz.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3vlkkfeka.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3ostfqvmv.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3eahpztlw.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3qkglqyuq.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3coopksfj.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3kiqclzib.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3xohumdtm.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3iotpeead.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3matqsdai.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3ngkargmz.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3qrgsywgi.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3nkynpknf.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3ehiijwlt.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3wdfppook.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3bohcwbfb.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3vggesmcx.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3swnqtput.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3kutmvflx.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3elwbulwb.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3omgtgllr.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3lvpvqgij.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3lhuxoqgn.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3mqywpyjg.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3avfpjatm.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3gxgzrdfa.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3wvioeilq.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3lovqptwo.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3zyabjwvj.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3dgbckrgn.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3fjhjhszc.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3oiwisxzs.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3sitobfyq.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3gviyqbey.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3jprzwkpb.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3uwhatlkr.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3wiotedal.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3xweogyzw.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3nabocjdn.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3ebdnbvck.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3ecwbtyws.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3ahekcjkr.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3fjvydtxt.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3kubymsqx.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3telqiwdy.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3vgqcogbb.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3pxhjqghu.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3xmbtjhjq.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3wpcvhvjh.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3wlhpymin.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3vfecjszc.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3ocfkimlv.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3zttppncq.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3mlbwzoir.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3rwdoxhfv.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3ampycpgb.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3bygilodw.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3faujalrc.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3daobqqdc.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3sxfqyjbc.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3cfuwwebj.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3lguvhelv.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3biutvlfo.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3gglrimfg.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3lrzsqavx.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3yclepjfv.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3epbavmxk.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3lgnqiepa.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3fxjvqhhj.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3rpsssihd.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3phgxiylv.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3yfnjvueg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pxqjwuei.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3kvalidoc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rpwlytsb.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3biwlkhig.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3aoaobbsd.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3pwgpdojx.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3mrxhijvn.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3nmwpxfak.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3dalpxfyq.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3smoxulgj.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3lwqtmarr.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3xtdvliwv.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3znabjcol.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3cdbfyozm.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3blggnwti.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3pzpfhkba.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3jxyszwcs.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3ffvvpomi.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3yvavtumu.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3dwxflxzb.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3mdadgfyx.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3gpfsrsfh.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3xorwhyxu.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3esbhryno.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3mbbcrnbd.html


<!-- 参考信息 -->