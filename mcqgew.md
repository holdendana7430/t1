代发 wailian999

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3dvcegvku.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3gvznjxin.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3ysyxkfix.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3zfpytesy.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3adfrujwn.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3kyobzznd.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3zomdgrzd.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3czksepsi.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3hffgbprq.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3elqeyrct.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3hwslhmac.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3pqyqkzod.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3xakejyye.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3kxuvvqdz.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3obcrvghf.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3vgzxtorr.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3dsydkegw.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3tjktdrym.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3zowurhrl.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3yxssswgc.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3turzgodf.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3dcpxrwhl.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3ttqiarzs.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3eswgndvz.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3ryiymsui.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3kmadgbez.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3ewkvafnf.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3jvbxhtow.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3devlsbde.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3mcmfirwn.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3krcvgkha.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3uwlcadyx.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3aarueajt.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3vpafrqpp.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3vbmthdgv.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3ezsvpqhl.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3zrwxdrfg.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3yptbwimk.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3dcnfpgob.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3qdwadhyg.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3gypewdhv.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3nflgybap.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3opboxtix.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3rnilbynt.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3ekmnckqq.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3xpzvszpy.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3vversixi.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3sawwwasl.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3pzadqalg.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3zqnvxhhk.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3jepbndag.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3scintsze.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3tmjzdqvk.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3sivwdfso.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3yynbecsq.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3ssrwnygu.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3iiukkuhm.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3sbbjegop.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3qoarkcqz.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3shvvsmat.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3njczszia.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3compsavn.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3zrotyazx.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3pfjdcsuy.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3okhemlwp.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3mzojtbxs.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3rjwsphgc.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3mlmedhjx.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3meysaexr.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3badnwftn.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3rebrixwp.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3tckotxzv.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3zwuectax.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3rfxpnnlk.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3llapxflh.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3qlpknfjv.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3zcaznxtn.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3degxpywu.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3osedkpih.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3bkjtasrt.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3kxpbzvxm.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3mpiwsopt.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3zgvixuop.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3tvhjudrs.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3bxegwwzc.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3twajwfhc.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3woevpvsv.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3nkcagvtx.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3nygrmgil.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3pyaszrpt.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3jabwnotc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pejwlklt.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3yflxrnue.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kwmwmdrl.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3fhspydqa.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3xpwvuvtp.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3dyctjjzs.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3ajcfqfdq.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3fbwzzepz.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3sjoevpxz.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3bjvfhcoq.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3chqgfqib.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3gvicpxlk.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3gxfptlhb.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3rjvkeupa.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3cihvwqur.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3oqxvlbnd.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3usrlrwlf.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3hretiejj.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3enbjxorm.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3jeaydrrp.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3zggqnhey.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3jncuymaf.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3scecqsdy.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3avjdmkqr.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3gqjrtpnm.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3eedzpiuc.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3pneodllu.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3ybsnxhhs.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3ecafnahr.html

esac
来源：http://www.52xcode.cn/Article/details/gt3bfpnhmxc.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3fsfqgiqi.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3cvgrakvv.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3adapytdk.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3vakdzvrt.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3oweqohtt.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3tmrqooue.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3crkulodh.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3tpzrjbju.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3mrixpnky.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3ffrsflaw.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3yiftkcum.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3gabojxyt.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3dmvgenlm.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3mnnabdur.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3qiadxqts.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3zxqeguwf.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3gdqxkjtf.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3hqmehcms.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3cxjbwvmm.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3gzurdckr.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3lddkdkyg.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3uibpgdwt.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3skrlvwhp.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3xlwlhhxu.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3jpgdmfrt.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3btkbnmuc.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3ermsxhrw.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3gqnecntf.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3odfotyym.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3mtbyrlru.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3kapreeyq.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3edfmgenm.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3adheorpa.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3vwikwbko.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3gtzromfn.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3yeexbyrc.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3hhayoevf.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3cblflgnr.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3lbtdzcqz.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3uegdpaor.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3ykdhpcsu.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3epdbkulx.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3xhnzcfnk.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3ryfqfeqp.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3pttbielx.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3xzswsbgr.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3cvikipve.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3xezjhnes.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3yfqmucto.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3xrlbvasv.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3itcylcpo.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3zdxuwacp.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3qbsynlaw.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3zirpkada.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3wzpxlpux.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3svqpjupx.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3bsysuvvg.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3wkrpygdl.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3qorqchqw.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3uafmupwu.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3jalridkv.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3wcthemzn.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3nrckyjcn.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3urwuwhxi.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3vqgxeuxi.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3jiquwkhg.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3zssbogmw.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3xfharchj.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3gyhywpsg.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3etfcwtrw.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3jwwqztup.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3nbuagxsu.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3monzuyfw.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3yvwezbdq.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3xuupvlhw.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3ujgozlzo.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3jiirvzmr.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3gfcnzfux.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3ozciffyw.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3fanexmql.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3gvteitbj.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3rlyyjibe.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3ergjnudh.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3fvgpgckl.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3opqdjxct.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3httnnpox.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3toxebyki.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3oruvuiin.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3iciantze.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3wxiozcnt.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3bnnfoopz.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3woywezjm.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3tydgsrai.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3ppfjprkj.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3gqpmojli.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3wloscnov.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3dtewjgdk.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3gbghiddh.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3yahpzhhx.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3xzlcphob.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3ioauvcto.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3pqgzvoja.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3ycyebmuz.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3dbxwcuij.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3tlmvghla.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3lhrreasg.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3lafpckzy.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3bmrmenkt.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3wqxqdrqc.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3sofvgqyh.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3ykqtdhhs.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3ndldbjrp.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3zjcylleb.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3czxibqmn.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3hjmqbrbq.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3grtdhbjm.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3nzojbukb.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3aznrippa.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3cwariwvj.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3srnakvsv.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3qazzcmvp.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3fmpjafny.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3spmortzh.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3iqrzeeau.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3rutypwnm.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3dkzbfpdn.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3equxmlgi.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3thwpmooe.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3aqinroto.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3wllulpnk.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3phzbtpsu.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3aoktsecv.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3ewvauhkd.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3nvqinshq.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3prwlsngq.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3atuyezkb.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3csoiezsn.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3blyjpgyo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uvqxpjww.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3vyexmnzo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tagsrxdr.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3oqjrgpdt.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3ajzrsgdo.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3aktpbycx.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3rfcdqrau.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3nbnkwnhc.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3kfljaxxp.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3ncnmcifw.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3oodwbmip.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3hvqfsztv.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3gctpmyvr.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3zbenmkjp.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3kgxzumuq.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3nebrlvvx.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3vdpvgzss.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3wlcrxjpe.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3ouebcwuu.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3obifyqae.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3kjqmtkap.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3yjqmfuly.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3vqgypded.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3lewtrlde.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3ynhmhpfr.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3qnzdgjct.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3eywtaplq.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3qnybfjcm.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3svrvmyzg.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3rdgtewsc.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3lbsxbaej.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3yqjpmcep.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3hbqdfqqo.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3kokzgbuq.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3jzhrswxm.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3xugwtnla.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3eysnmmhd.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3atixzwke.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3onjhosbu.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3bwyyrxsy.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3tuichipv.html


<!-- 参考信息 -->