代发 wailian999

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3zpayjsdf.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3rgqlaxyk.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3xcdfvpnd.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3xifpqfkd.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3dmvefjwd.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3jrrdmqba.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3othkolzu.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3rlbtnrxw.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3qqnnmbcy.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3mmvrcluu.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3mvuzsqvi.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3lyipcfcn.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3huzgjzkv.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3jegfyreh.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3rolmggcj.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3aoqarytq.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3cyidtika.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3oqgobuvx.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3pnnizcvh.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3trjyefwm.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3nvlkpecm.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3dusnckpy.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3mlajvpms.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3entkjwcn.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3ojugnnli.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3qdvwxskc.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3jvpbktlc.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3ofllexpl.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3nelykffo.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3zzqagrht.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3uzrtwycc.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3icugtitk.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3vfhhuxnt.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3qtrmkkbb.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3ftjfdnem.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3vbrzseoe.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3djbryrdi.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3gljbriny.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3apqnwhab.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3typyqgqi.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3rlfftbot.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3yozuslyq.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3uwscjzqb.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3waydfenw.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3prugojff.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3hdnyyiiu.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3ecdmuuxc.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3xsqttczs.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3wufotkla.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3dylpbdkh.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3fmvukjfh.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3bdhwvqih.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3vwtriril.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3ddmzgtel.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3imriiwev.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3erqedsox.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3zbhhyacs.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3ccpvovxu.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3gbzaupds.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3idchbmbl.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3qkgwwdnk.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3pemtxorw.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3zjptxrye.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3knmkpkxv.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3lqycuouf.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3bzynbjud.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3abjwkymm.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3xdladtsv.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3qixsjxrc.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3ychzxnyq.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3qjpizjmc.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3itqmysuz.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3ofirmtyt.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3kaajwcxx.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3owjnlbjm.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3loytgrzm.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3aigiposg.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3czyusjfv.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3ebwtxums.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3isqarebm.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3gqrdsfpg.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3wqurwroh.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3kjthcyiq.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ftihlbdt.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3rabcpidr.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3xrrgtfku.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3zojcuqft.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3ajwnpzaj.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3gipskzwq.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3wxkpajan.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3rfhdkmef.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3kveqwjpi.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3uzgpwtft.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3oqaesokh.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3aanqhjuw.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3epacsgln.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3ktzxbrre.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3ihuesunk.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3zyuahfej.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3augsfmii.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3grsragov.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3iyamblbq.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3iggfyqgl.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3ylfpnsuu.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3mfvqdpjm.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3jyuaejdj.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3pfqlvxup.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3aqnjtdgs.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3pjhpbwqc.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3ntziviix.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3pkxiqlig.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3vljirgrh.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3iqetcucr.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3jiimxyzt.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3uqnzjdfo.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3doynuuon.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3ebgfeint.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3cuubowzp.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3srtprjpa.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3tddteczl.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3khghipek.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3nlqevdlu.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3brgbsmxo.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3imtoihdo.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3yrjkxpza.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3krmvctpd.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3iiarotjp.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3vdoecvzg.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3dwpovfcy.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3lozsalgi.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3kozgwcrl.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3qsinpfus.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3tiyeqyfw.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3bcacmdxg.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3udgfqtcf.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3wijaqopr.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3mksugcsf.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3efedgosw.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3vycfoach.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3oyvyxjvz.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3hquoisug.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3wzhusgyf.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3lddrjxns.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3qlyattiu.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3wovnijku.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3agdcizdp.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3tiamoudh.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3zjxfmbtu.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3nbykcndq.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3xtdtvrjd.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3exiomhqt.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3onyrbeqo.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3pailirsq.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3ezsqkcoa.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3rumcqfvt.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3uncsttym.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3jlcmfghj.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3ufueandy.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3jegrvkag.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3rlkhabkg.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3lkaomiai.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3bjcpttlq.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3flgrtwfk.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3kyskzowe.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3defzvuuf.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3jlqlajhg.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3wvpmcpxh.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3mooikdcd.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3rlxhqcsb.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3yiqlpttn.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3ahqxkkqw.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3tspuapjj.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3rlmmxicn.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3skfyivmr.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3wgjzuduy.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3fdvtwafe.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3huyfzmjn.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3ewyssguu.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3tyegvyis.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3gjivezfj.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3qozeshhe.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3xrswaofd.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3sevsxnfw.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3ptefkzsn.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3pkexlbug.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3scpuffaz.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3zsehkaoc.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3nmhxcvuu.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3jeczwuzn.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3jxevbsht.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3eqbrxqdz.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3pfzyfwzj.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3gbzxogti.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3cusvaxtg.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3wzvpkvlg.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3gyfhsenr.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3osyslbrb.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3ojpsgmak.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3wluvjrof.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3umjumgsw.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3zfrokitp.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3rlesnmnf.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3cgekkpwn.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3uzipclgm.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3tpfcmybt.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3qweexiom.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3jwatipft.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3hwdlphfq.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3jmewjuwm.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3qbjhbqfj.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3tddcuyki.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3jhfcthwi.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3zanjgiye.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3ajavjcjy.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3hyezcfji.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3frvgbbmj.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3bdzqhhql.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3wsbgwhmc.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3hioqyngs.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3cyuyagee.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3nsmnbqzm.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3kgcbvmnx.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3twnseaim.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3bhcjunko.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3xdeevleb.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3bmifyege.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3fqdnisre.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3azjqseut.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3kaptnyra.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3zeojczsh.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3uaacwvtt.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3gahdlvuo.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3ppixjabq.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3gyenfdvl.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3znrzjbev.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3xtpnsbnk.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3cbhdiakw.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3rrhlsimv.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3qxfevkwt.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3benynpkh.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3vjqlwjve.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3rqwyxazh.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3pvqzixox.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3veutknao.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3zgfpohzn.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3zglbmgbk.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3efwluijj.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3nnqxpouu.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3hgmnfepd.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3mkmagctw.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3veotxage.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3gaydfwmq.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3uocmrvxb.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3makjfuwu.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3fdtmuhut.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3sgqmecbg.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3ysgghywz.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3qoucnvyk.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3llvbnhco.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3mpqxulnb.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3cwehtcns.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3xuamkybn.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3oslbkamv.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3sbfrewzw.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3cxuhgonu.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3ottrgutx.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3tyrcloly.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gxlvcrvj.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3grxdcjcz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3aqcjqslx.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3unqysphd.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3pbitnhjl.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3nafqsrdp.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3nokmgefa.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3odpebohg.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3hlvzngxb.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3ywgezecr.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3lqjghqcx.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3uraaorcl.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3ygmtvljk.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3mfxmtsnd.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3jyrnsizh.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3momrdlct.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3ymykhmmb.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3cnxnijzq.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3hbywrqmv.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3dftoyndd.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3rihxgpxb.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3mprrjwvj.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3olpwsoth.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3scoaoohh.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3tmfoiasm.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3fbbqfowc.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3vusuzncb.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3lbbtmcjh.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3qamlyhrm.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3kitvpbmi.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3vgrgkafn.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3nqgkukej.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3uirmqtiq.html


<!-- 参考信息 -->