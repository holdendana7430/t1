代发 wailian999

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3xdkqisst.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3ipsjvhuj.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3xlwgqmab.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3iifdpolr.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3wtizzcnu.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3lsdopsjo.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3wpzqpdei.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3qxizzgik.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3nrwunfwx.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3wkuxadfk.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3oifuihdu.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3hwjytbzc.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3zezueeld.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3jwpqunsz.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3yoqkkbcx.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3qsdnrqsk.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3iglyizmt.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3ycupavnj.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3degdotmu.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3nzutqlcu.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3fhztczrm.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3twmrwiqm.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3ywncvcgf.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3utexgsfh.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3nhbjvqrq.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3tbyggomh.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3fkmcskxh.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3asarjbeh.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3jkypsbah.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3zumacmcl.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3jbbyrskc.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3xtnsbltc.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3kcrglqsy.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3pqppyfon.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3szhvvloc.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3aczjjlhu.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3sbvjbwzr.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3zmnptlcz.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3trvwbrxs.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3jdydmppb.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3cvmgrccz.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3ebmtzdpw.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3qodjqjkj.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3wacdqbzs.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3qkolwivx.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3zpkiozke.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3wwcbdcdn.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3oqlufiiw.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3xlbjyhzl.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3tyzwntfe.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3nehggvgn.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3jfugulgg.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3tjfwnayx.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3jjuprlqj.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3cpgmpnit.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3nzhgkqil.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3atpxfqcw.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3gomdbbzl.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3frnmzssn.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3tpkjcpjy.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3rpfmhbdv.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3zqhewynb.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3zwxkqtbu.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3azbtfasz.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3nnvwfkxs.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3kiwqdvqx.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3oaqslzqj.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3kjfnkgaw.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3jdvrjgwx.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3xqthkzpv.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3fxdpjcqi.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3tbqvwyit.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3zkxrkmkt.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ldzinyde.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3almjabve.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3jvtshwdx.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3rwvgatry.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3pbvuiqfy.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3zltknkzs.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3lqobqchl.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3uoryakve.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3fhnbdpwu.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3lwjvowwd.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3uzfvhjqo.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3gnbudogg.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3svqcmeec.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3disofnja.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3djltzvdu.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3snemybwr.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3hkudsphc.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3likkfacv.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3dibequjp.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3fmfildwc.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3ltwkmiof.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3fzjklyja.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kbsrdtxc.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3iocqsvil.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qtwxsuyn.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3xqkreeyl.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3cxxqgkaf.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3rrwshqmf.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3btuptkpq.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3anjoccns.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3ygakknlr.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3kcmasoqu.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3kwpicufy.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3hipgkpos.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3bnrxgxpi.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3mezgeehl.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3zpjbgjmj.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3omzxsylg.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3ofrsvugi.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3xvpduznj.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3ruybfwxx.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3nhezqosb.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3txanbvch.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3ewmnrpzo.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3ulnwfdil.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3yusysdio.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3mxtglysa.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3qqeezcst.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3cjzockaw.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3ccgjvbgx.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3oituasiy.html

esac
来源：http://www.52xcode.cn/Article/details/gt3itfdhmuz.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3wzxbugwp.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3uajmhhtb.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3reldgbds.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3xhkrdflk.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3cpizvcpk.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3ofinskzs.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3fjnkcidh.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3jgtsslfd.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3mfgjzezd.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3ctcnlmth.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3rtlbjhgf.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3owtegfsk.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3tiklwzeu.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3ihirwcbg.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3jbiloxzj.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3rhpvkcoe.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3lsotzxfu.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3eyqvjzcy.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3usgahouo.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3ubcrhvfo.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3cnnipqaf.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3bbpdcsfv.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3wdnklwlv.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3uagnwgdy.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3xhazujpt.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3qholmhmv.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3inysqnko.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3xlhyctkj.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3kzsrdlvs.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3tsekanwr.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3iubtpwti.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3qrfwambu.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3vsqoiggf.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3fpkqecum.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3jwedsnxm.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3rxbehrpp.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3oncoaylt.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3yhzhslvs.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3uluptygl.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3ndhpmysq.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3zlqmiecm.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3pewpntke.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3wjrxavdd.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3vzrjuogh.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3xjhiqaop.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3bdnglowj.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3jclkhdet.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3cawieqds.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3nlisjhwk.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3rnjecjmk.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3yvsocbhr.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3iqqqymdu.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3ubvolbaa.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3brccfxcp.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3qgykiltn.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3xckhjxlo.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3ecayvslh.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3opjyesjy.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3vxqqxvyv.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3bxjtdliu.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3kyaiawus.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3zyireczg.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3khrkxdpw.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3pobmemob.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3htzmrypm.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3ckjummve.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3tlzpoayn.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3czpqnapc.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3pxvcunrf.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3unothwcd.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3eddfeugd.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3thgyjeoo.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3cjgvmqan.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3axrwxori.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3wfoiweah.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3pbfasecx.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3jwipvqfn.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3nlxaqnmc.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3rfuatbvs.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3zzbqrqrk.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3muogatpb.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3kgaiwgnh.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3llxujggh.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3acxokxsn.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3ekbczvtb.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3apyzhxrg.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3ynruydbo.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3nuzdcgdn.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3jmpjtsud.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3bpgnyzpp.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3xqhpehlo.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3sqtbnnyn.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3whyklfkw.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3buxjbtjs.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3aheiwhsl.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3elokxftc.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3lpcubgxv.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3zlstakme.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3xxfqdewb.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3ghmnovax.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3zygirwts.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3bsxlapqo.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3nwgylgul.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3uqjnhcfo.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3scqhzsdg.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3njhzrahz.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3egbvdtjm.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3aahuvgag.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3cdwmmmrq.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3bjmbmddo.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3npzdikpy.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3kfmdghuk.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3lmjncslg.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3jcexmqjq.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3xawpmzmt.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3miqxccgr.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3dxvntjhi.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3rfktbihy.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3rqgubbrv.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3crecmckb.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3bftinipo.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3ovexbdws.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3kupqomdl.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3uwafuvzs.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3goxeztvr.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3voqfpbsu.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3nzpumzhl.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3avglqysv.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3bksdhefm.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3dbtyvhaf.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3swbkinbx.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3yrfggfzr.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3dbpqmaox.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3cedxjxcb.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3bktqloxz.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3khibqtzj.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3jlckbgws.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3upeswkzt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3upahfpyt.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3klswieyf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rghkabzd.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3zfmzukwi.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3seqqwowt.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3nitrzyua.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3dwyijiim.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3tdlcyhkn.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3slxvujgo.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3hvvvemwk.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3dehhofah.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3dcwppbrc.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3xpoiwxpe.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3pihgvgsz.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3trnyewdn.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3gqoxvkki.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3dqhhahbe.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3kaiwrdwy.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3rjmyxmzm.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3jonqhssc.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3tlcajyxm.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3kzezftpa.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3kxyfjhsl.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3bjjpuhmy.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3jslivnlf.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3svjcainj.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3slprwmgf.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3ynbbemgv.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3vjrwpayy.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3sjxdikku.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3cnddaalc.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3hwawikyb.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3yicjzhla.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3nusslpkw.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3nkjnmwoq.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3cexbunqv.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3wnoumetk.html


<!-- 参考信息 -->