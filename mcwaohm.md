代发 wailian999

SELECT u.name, o.amount FROM users u
来源：http://m.share.zdbjq.cn/Article/details/gudfmsmvc.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wap.zdbjq.cn/Article/details/gutysrlrt.sHtML

[Q43] 标量子查询
来源：http://www.m.share.hesvh.cn/Article/details/gwfijftgs.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://blog.zdbjq.cn/Article/details/gmqjvojjv.sHtML

[Q44] IN 子查询
来源：http://www.blog.zdbjq.cn/Article/details/gkudcbhft.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://blog.zdbjq.cn/Article/details/grxfobinn.sHtML

[Q45] EXISTS 判断存在
来源：http://mobile.zdbjq.cn/Article/details/gabmgrsve.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.zdbjq.cn/Article/details/gfvfaeerj.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://3g.zdbjq.cn/Article/details/gxxetnwrl.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.zdbjq.cn/Article/details/gulitnpqx.sHtML

[Q47] 与平均值比较
来源：http://mobile.hesvh.cn/Article/details/gzruumqkm.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.share.fehbvm.com/Article/details/gygtfdlwl.sHtML

[Q48] CTE 公用表表达式
来源：http://m.share.hesvh.cn/Article/details/gahslmbei.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.m.share.hesvh.cn/Article/details/gngvaqato.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.m.share.zdbjq.cn/Article/details/gycjmtyqt.sHtML

[Q49] 更新单行
来源：http://www.m.share.zdbjq.cn/Article/details/gjvufcvcb.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://baike.hesvh.cn/Article/details/gwacnqfmy.sHtML

[Q50] 批量更新
来源：http://www.share.zdbjq.cn/Article/details/gvwrgniiv.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mobile.zdbjq.cn/Article/details/gmxvnsqmz.sHtML

[Q51] 用子查询更新
来源：http://www.share.fehbvm.com/Article/details/gppsmpppf.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mobile.hesvh.cn/Article/details/gfsrentnl.sHtML

[Q52] 删除指定行
来源：http://baike.zdbjq.cn/Article/details/gssrnvjpw.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.blog.hesvh.cn/Article/details/gqmjujyjq.sHtML

[Q53] 按条件删除
来源：http://baike.hesvh.cn/Article/details/gfxtuples.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://read.share.hesvh.cn/Article/details/gqystcean.sHtML

[Q54] 清空表
来源：http://www.m.share.zdbjq.cn/Article/details/ggvpiliho.sHtML

TRUNCATE TABLE logs;
来源：http://wap.zdbjq.cn/Article/details/glimufdjg.sHtML

[Q55] 排名（并列占位）
来源：http://read.share.fehbvm.com/Article/details/gjkbjqgtp.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://3g.hesvh.cn/Article/details/gjhxwvntb.sHtML

[Q56] 密集排名（并列不占位）
来源：http://read.share.hesvh.cn/Article/details/gxthdkmac.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://baike.hesvh.cn/Article/details/gdvgpzwdx.sHtML

[Q57] 行号
来源：http://www.share.hesvh.cn/Article/details/gjwjiuaqv.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://3g.fehbvm.com/Article/details/gzizjajyu.sHtML

[Q58] 累计求和
来源：http://www.share.hesvh.cn/Article/details/gcjtxwgtw.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/gvggbygjz.sHtML

[Q59] 分组内累计
来源：http://read.share.fehbvm.com/Article/details/gweuvphjl.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/gfvhpjlwu.sHtML

[Q60] 取上一行 / 下一行
来源：http://baike.hesvh.cn/Article/details/gdjklaeru.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://3g.zdbjq.cn/Article/details/gdqkvedvf.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mobile.fehbvm.com/Article/details/gjzwjhtsk.sHtML

[Q61] 移动平均
来源：http://3g.hesvh.cn/Article/details/gcvkwvjln.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://3g.fehbvm.com/Article/details/gugauacaq.sHtML

[Q62] 分组占比
来源：http://www.share.fehbvm.com/Article/details/gacaipqga.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://3g.hesvh.cn/Article/details/gjjssrhjc.sHtML

[Q63] 开启事务
来源：http://3g.zdbjq.cn/Article/details/gcvbwjkal.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.zdbjq.cn/Article/details/gbmsirstf.sHtML

[Q64] 提交事务
来源：http://3g.fehbvm.com/Article/details/guwgpphou.sHtML

COMMIT;
来源：http://blog.hesvh.cn/Article/details/giqkgtiys.sHtML

[Q65] 回滚事务
来源：http://wap.hesvh.cn/Article/details/gfkhbtwkp.sHtML

ROLLBACK;
来源：http://read.share.fehbvm.com/Article/details/gqhncbanh.sHtML

[Q66] 行锁查询
来源：http://www.m.share.zdbjq.cn/Article/details/ggoiruxau.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.m.share.zdbjq.cn/Article/details/gkgnyqpbh.sHtML

[Q67] 设置隔离级别
来源：http://www.blog.hesvh.cn/Article/details/gmkpfhytv.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.blog.hesvh.cn/Article/details/gyutzwrva.sHtML

[Q68] 保存点
来源：http://mobile.fehbvm.com/Article/details/gtddgjzdr.sHtML

SAVEPOINT sp1;
来源：http://m.share.hesvh.cn/Article/details/gflqqdxxr.sHtML

ROLLBACK TO sp1;
来源：http://baike.hesvh.cn/Article/details/ganlvhzkd.sHtML

[Q69] 查看执行计划
来源：http://baike.fehbvm.com/Article/details/ghcjkcnem.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://blog.zdbjq.cn/Article/details/gmndvathv.sHtML

[Q70] 更新统计信息
来源：http://www.share.zdbjq.cn/Article/details/gnoavjoud.sHtML

ANALYZE TABLE users;
来源：http://3g.hesvh.cn/Article/details/gbcjzkvfj.sHtML

[Q71] 查看建表语句
来源：http://m.share.zdbjq.cn/Article/details/gqbacqcuq.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.fehbvm.com/Article/details/gapyrwhhs.sHtML

[Q72] 查看索引
来源：http://m.share.hesvh.cn/Article/details/gtgymxqtl.sHtML

SHOW INDEX FROM users;
来源：http://blog.fehbvm.com/Article/details/grzzjxthd.sHtML

[Q73] 查看表状态
来源：http://mobile.fehbvm.com/Article/details/gnheuutjy.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://3g.fehbvm.com/Article/details/gpanbxmue.sHtML

[Q74] 强制使用索引
来源：http://blog.zdbjq.cn/Article/details/gcunubyqw.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.fehbvm.com/Article/details/gsemewbla.sHtML

[Q75] 日期格式化
来源：http://baike.fehbvm.com/Article/details/gmyqtwxuo.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://blog.fehbvm.com/Article/details/gesgjmpvf.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.zdbjq.cn/Article/details/gamplffvj.sHtML

[Q76] 按天统计
来源：http://m.share.hesvh.cn/Article/details/gsxpktkxz.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://blog.hesvh.cn/Article/details/gajxmflub.sHtML

[Q77] 时间加减
来源：http://www.blog.hesvh.cn/Article/details/gfyhrouoy.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://3g.zdbjq.cn/Article/details/grnmzmwsn.sHtML

[Q78] 当前时间
来源：http://read.share.zdbjq.cn/Article/details/gpkexunna.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wap.zdbjq.cn/Article/details/gsjcduiod.sHtML

[Q79] 字符串拼接
来源：http://mobile.zdbjq.cn/Article/details/gqzoydxvw.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://blog.fehbvm.com/Article/details/geldruyve.sHtML

[Q80] 字符串截取
来源：http://m.share.zdbjq.cn/Article/details/gtrgrfbll.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wap.hesvh.cn/Article/details/gegmhlrcx.sHtML

[Q81] 字符串替换
来源：http://blog.zdbjq.cn/Article/details/gjsbzxbiu.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gshubzpiy.sHtML

[Q82] 字符长度与字节长度
来源：http://blog.zdbjq.cn/Article/details/gzgtadjxo.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/goxrrykxg.sHtML

[Q83] 大小写转换
来源：http://wap.hesvh.cn/Article/details/gzdfvldge.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gwbwtrujz.sHtML

[Q84] 去除首尾空格
来源：http://baike.zdbjq.cn/Article/details/gjoktkzmz.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.hesvh.cn/Article/details/gpkfjoeyc.sHtML

[Q85] 数值取整
来源：http://mobile.zdbjq.cn/Article/details/guogndyrh.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.share.fehbvm.com/Article/details/gwqimwghh.sHtML

[Q86] 读取 JSON 字段
来源：http://3g.hesvh.cn/Article/details/glhfucnqu.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.zdbjq.cn/Article/details/gsyoybhkd.sHtML

[Q87] JSON 字段做条件
来源：http://read.share.fehbvm.com/Article/details/ggtzwqtgd.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.zdbjq.cn/Article/details/gbkdyslkn.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.m.share.zdbjq.cn/Article/details/gdlonvgga.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.hesvh.cn/Article/details/gerjkbexc.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://baike.zdbjq.cn/Article/details/ghgzargmn.sHtML

[Q89] 判断表是否存在
来源：http://read.share.hesvh.cn/Article/details/ggexkfmoy.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.fehbvm.com/Article/details/gqcskvjdy.sHtML

[Q90] 生成序号列
来源：http://www.share.fehbvm.com/Article/details/gtougpboi.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.share.hesvh.cn/Article/details/grtjnxfmi.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gpwkwpdoh.sHtML

R. Bash 专题
来源：http://www.share.hesvh.cn/Article/details/gakpchoaz.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gvlogpmrj.sHtML

[R01] shebang 与严格模式
来源：http://www.m.share.zdbjq.cn/Article/details/gxpzxmhze.sHtML

#!/usr/bin/env bash
来源：http://wap.zdbjq.cn/Article/details/ggzukiqlo.sHtML

set -euo pipefail
来源：http://www.m.share.fehbvm.com/Article/details/gewbnhmok.sHtML

[R02] 变量赋值与使用
来源：http://3g.zdbjq.cn/Article/details/gpvrzprbs.sHtML

name="Tom"; echo "$name"
来源：http://www.share.fehbvm.com/Article/details/guhyqslyy.sHtML

[R03] 只读变量
来源：http://baike.hesvh.cn/Article/details/gfbridaor.sHtML

readonly PI=3.14
来源：http://blog.hesvh.cn/Article/details/gghnkhvic.sHtML

[R04] 位置参数
来源：http://m.share.zdbjq.cn/Article/details/gzfkvwymu.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.zdbjq.cn/Article/details/gyzljtzib.sHtML

[R05] 参数默认值
来源：http://m.share.zdbjq.cn/Article/details/gyehndpfw.sHtML

name="${1:-default}"
来源：http://read.share.zdbjq.cn/Article/details/gqrntrqsp.sHtML

[R06] 判断命令是否存在
来源：http://blog.fehbvm.com/Article/details/gohjydpul.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.zdbjq.cn/Article/details/gpbqtnhkc.sHtML

[R07] if 判断文件
来源：http://m.share.zdbjq.cn/Article/details/glbmkgnxu.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.fehbvm.com/Article/details/gvewywtkn.sHtML

[R08] 数值比较
来源：http://mobile.zdbjq.cn/Article/details/gmbkkddye.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://m.share.zdbjq.cn/Article/details/gnhfwquhe.sHtML

[R09] 字符串比较
来源：http://read.share.fehbvm.com/Article/details/gnzwjjomk.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.fehbvm.com/Article/details/gzhdixhku.sHtML

[R10] 正则匹配
来源：http://read.share.zdbjq.cn/Article/details/gwtfeybdd.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://read.share.zdbjq.cn/Article/details/gywmxclne.sHtML

[R11] case 多分支
来源：http://m.share.zdbjq.cn/Article/details/geqsdflmb.sHtML

case "$1" in
来源：http://blog.zdbjq.cn/Article/details/gncnylhvk.sHtML

start) echo "启动" ;;
来源：http://blog.zdbjq.cn/Article/details/gqldqynyx.sHtML

stop)  echo "停止" ;;
来源：http://www.share.hesvh.cn/Article/details/gdpatvjng.sHtML

*)     echo "未知命令" ;;
来源：http://wap.hesvh.cn/Article/details/ghfrmkeul.sHtML

esac
来源：http://www.share.fehbvm.com/Article/details/gppxtivvr.sHtML

[R12] for 遍历文件
来源：http://m.share.hesvh.cn/Article/details/gijgjbeen.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.fehbvm.com/Article/details/gmykwtzzv.sHtML

[R13] for 计数循环
来源：http://baike.zdbjq.cn/Article/details/geinsajct.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.hesvh.cn/Article/details/gjbmgswjb.sHtML

[R14] C 风格 for
来源：http://m.share.zdbjq.cn/Article/details/glbehmwgi.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wap.zdbjq.cn/Article/details/gexrviall.sHtML

[R15] while 逐行读文件
来源：http://m.share.zdbjq.cn/Article/details/ghhtthcuj.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.zdbjq.cn/Article/details/gizyfbfra.sHtML

[R16] until 等待条件
来源：http://read.share.fehbvm.com/Article/details/gwbpbdcgy.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.share.zdbjq.cn/Article/details/ghtryyucr.sHtML

[R17] 数组定义与取值
来源：http://blog.hesvh.cn/Article/details/gqzzborea.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.hesvh.cn/Article/details/gmsldyztk.sHtML

[R18] 遍历数组
来源：http://mobile.hesvh.cn/Article/details/giiwqrisw.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.fehbvm.com/Article/details/ghwuyfmpq.sHtML

[R19] 数组长度
来源：http://blog.hesvh.cn/Article/details/gwkrhzrmu.sHtML

echo "${#arr[@]}"
来源：http://m.share.fehbvm.com/Article/details/gjycfrjns.sHtML

[R20] 关联数组（字典）
来源：http://baike.hesvh.cn/Article/details/ggvnhounl.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.hesvh.cn/Article/details/gobnecaex.sHtML

[R21] 字符串长度
来源：http://m.share.hesvh.cn/Article/details/gzvqgrmqy.sHtML

echo "${#s}"
来源：http://www.m.share.fehbvm.com/Article/details/gumbuxiyg.sHtML

[R22] 截取子串
来源：http://3g.fehbvm.com/Article/details/gtyjaoxsc.sHtML

echo "${s:0:5}"
来源：http://blog.zdbjq.cn/Article/details/gyhvrlpwl.sHtML

[R23] 字符串替换
来源：http://www.m.share.fehbvm.com/Article/details/gfnciwcuf.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.fehbvm.com/Article/details/gnqlajnnt.sHtML

[R24] 大小写转换
来源：http://www.blog.zdbjq.cn/Article/details/gidsuoqpi.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.fehbvm.com/Article/details/gflwxesvy.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.hesvh.cn/Article/details/gzlpbetix.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.hesvh.cn/Article/details/gwjvemkwg.sHtML

[R26] 命令替换
来源：http://www.share.zdbjq.cn/Article/details/gggvagxaj.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.zdbjq.cn/Article/details/ghyxkzomq.sHtML

[R27] 算术展开
来源：http://wap.zdbjq.cn/Article/details/gpvihuhnx.sHtML

echo $((1 + 2 * 3))
来源：http://3g.hesvh.cn/Article/details/gufrmlzok.sHtML

[R28] 浮点运算
来源：http://blog.hesvh.cn/Article/details/gmbegmlse.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.zdbjq.cn/Article/details/gpgoklbxl.sHtML

[R29] 定义函数
来源：http://baike.hesvh.cn/Article/details/gugfeiymj.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.fehbvm.com/Article/details/gnfobghal.sHtML

[R30] 函数返回状态码
来源：http://mobile.zdbjq.cn/Article/details/gdjtajgdo.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.fehbvm.com/Article/details/gmtxvpwgo.sHtML

[R31] 局部变量
来源：http://m.share.fehbvm.com/Article/details/grtbvpdxc.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.zdbjq.cn/Article/details/gkykezonu.sHtML

[R32] 参数个数校验
来源：http://www.share.fehbvm.com/Article/details/gkrhfypqz.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.zdbjq.cn/Article/details/gmiculfia.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.hesvh.cn/Article/details/gzoiibicn.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.hesvh.cn/Article/details/ghxzhgibu.sHtML

[R34] 退出时清理
来源：http://read.share.zdbjq.cn/Article/details/gtlrzkcqu.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.hesvh.cn/Article/details/gwjjjhezg.sHtML

[R35] 后台执行并等待
来源：http://m.share.zdbjq.cn/Article/details/ginjrrrkn.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.hesvh.cn/Article/details/gfvwslqma.sHtML

[R36] 并发执行多个任务
来源：http://baike.fehbvm.com/Article/details/gcffkfwqi.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.zdbjq.cn/Article/details/gddokrfig.sHtML

[R37] 把输出赋给变量
来源：http://baike.hesvh.cn/Article/details/gnuotaexc.sHtML

files=$(ls -1)
来源：http://blog.hesvh.cn/Article/details/gqfjvwghj.sHtML

[R38] 管道串联
来源：http://www.m.share.fehbvm.com/Article/details/ggizpborm.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.zdbjq.cn/Article/details/gvuopgliy.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.hesvh.cn/Article/details/ginubmbvc.sHtML

cmd > out.log 2>&1
来源：http://blog.fehbvm.com/Article/details/gsdgejulv.sHtML

[R40] 追加写日志
来源：http://www.m.share.zdbjq.cn/Article/details/gxtbuuchf.sHtML

echo "log" >> out.log
来源：http://www.blog.fehbvm.com/Article/details/grecgppvr.sHtML

[R41] 丢弃输出
来源：http://read.share.zdbjq.cn/Article/details/gexlcbzeo.sHtML

cmd >/dev/null 2>&1
来源：http://baike.hesvh.cn/Article/details/gponzjpaa.sHtML

[R42] 输入重定向
来源：http://3g.hesvh.cn/Article/details/gewjgsjyu.sHtML

wc -l < a.txt
来源：http://mobile.zdbjq.cn/Article/details/gcydrvtry.sHtML

[R43] 按名字查找文件
来源：http://m.share.hesvh.cn/Article/details/gpwldmakb.sHtML

find . -name "*.log" -type f
来源：http://read.share.hesvh.cn/Article/details/gtgiiurty.sHtML

[R44] 按修改时间查找
来源：http://baike.zdbjq.cn/Article/details/guuiexcjr.sHtML

find . -mtime -7 -type f
来源：http://read.share.zdbjq.cn/Article/details/glwmidlqt.sHtML

[R45] 批量删除
来源：http://www.share.fehbvm.com/Article/details/ghtmcznab.sHtML

find . -name "*.tmp" -delete
来源：http://baike.fehbvm.com/Article/details/gprujfnyr.sHtML

[R46] 递归替换文件内容
来源：http://read.share.hesvh.cn/Article/details/gyieuojpy.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.zdbjq.cn/Article/details/gtcrllgnl.sHtML

[R47] sed 单行替换
来源：http://3g.fehbvm.com/Article/details/gbklpihcd.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.hesvh.cn/Article/details/gmvabttwo.sHtML

[R48] awk 取指定列
来源：http://wap.hesvh.cn/Article/details/gznehvuyv.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.fehbvm.com/Article/details/grxolxqqz.sHtML

[R49] awk 带条件
来源：http://blog.fehbvm.com/Article/details/gimfhwmen.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.zdbjq.cn/Article/details/gunoeotao.sHtML

[R50] awk 求和
来源：http://wap.zdbjq.cn/Article/details/gftdqdadh.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.hesvh.cn/Article/details/gbvpcagqb.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.fehbvm.com/Article/details/gdizmnqtu.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.fehbvm.com/Article/details/gcfxegnmu.sHtML

[R52] 统计行数
来源：http://baike.fehbvm.com/Article/details/gynceurul.sHtML

wc -l a.txt
来源：http://wap.zdbjq.cn/Article/details/gieeeuvuk.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.hesvh.cn/Article/details/gruqxwrym.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.fehbvm.com/Article/details/gmztawvjm.sHtML

[R54] 比较两个文件
来源：http://mobile.fehbvm.com/Article/details/gjfqypvbe.sHtML

diff a.txt b.txt
来源：http://www.blog.zdbjq.cn/Article/details/guqxwrcun.sHtML

[R55] 压缩与解压
来源：http://3g.zdbjq.cn/Article/details/ggjftxdcf.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.fehbvm.com/Article/details/gfzhgapqd.sHtML

[R56] 远程拷贝
来源：http://3g.zdbjq.cn/Article/details/gqygyicpd.sHtML

scp file user@host:/path/
来源：http://read.share.zdbjq.cn/Article/details/gfdrnqlxl.sHtML

[R57] 远程执行命令
来源：http://3g.zdbjq.cn/Article/details/gmtgxzmjv.sHtML

ssh user@host 'uptime'
来源：http://mobile.zdbjq.cn/Article/details/gtdifbqeh.sHtML

[R58] 下载文件
来源：http://www.blog.fehbvm.com/Article/details/gvnsmdgml.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.zdbjq.cn/Article/details/gorqjyefv.sHtML

[R59] 发 POST JSON
来源：http://www.share.hesvh.cn/Article/details/ggomlakxi.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.fehbvm.com/Article/details/ghffbdadm.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.hesvh.cn/Article/details/gumrapeai.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.fehbvm.com/Article/details/gqjlcmkpa.sHtML

[R61] 磁盘占用
来源：http://www.m.share.hesvh.cn/Article/details/gjbptrikh.sHtML

df -h;  du -sh *
来源：http://www.m.share.fehbvm.com/Article/details/gdwprqazl.sHtML

[R62] 找最占空间的文件
来源：http://m.share.zdbjq.cn/Article/details/glkdyneaa.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.zdbjq.cn/Article/details/gruigviau.sHtML

[R63] 内存与进程
来源：http://read.share.hesvh.cn/Article/details/gnycbydwn.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.hesvh.cn/Article/details/gbjlqhzbd.sHtML

[R64] 结束进程
来源：http://baike.hesvh.cn/Article/details/gyxxrvgbd.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.fehbvm.com/Article/details/gucccuipb.sHtML

[R65] 查看端口占用
来源：http://m.share.hesvh.cn/Article/details/gmzuxyhmf.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.hesvh.cn/Article/details/gptyqcthv.sHtML

[R66] 定时任务
来源：http://baike.hesvh.cn/Article/details/gngbhrpua.sHtML

crontab -e;  crontab -l
来源：http://baike.fehbvm.com/Article/details/girwbcrfs.sHtML

[R67] 生成随机十六进制串
来源：http://3g.fehbvm.com/Article/details/gfhxzlxys.sHtML

openssl rand -hex 16
来源：http://www.m.share.hesvh.cn/Article/details/gmppdjuyo.sHtML

[R68] 计算文件校验值
来源：http://mobile.fehbvm.com/Article/details/guxxpmbdv.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.hesvh.cn/Article/details/gssfwddqa.sHtML

[R69] 生成随机密码
来源：http://mobile.hesvh.cn/Article/details/gjbakuzut.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.zdbjq.cn/Article/details/gqtrlxqpx.sHtML

[R70] 时间戳与互转
来源：http://blog.hesvh.cn/Article/details/gedxnexkg.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.hesvh.cn/Article/details/gvkrncqhk.sHtML

[R71] 日期格式化
来源：http://read.share.fehbvm.com/Article/details/gmtdeceul.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.fehbvm.com/Article/details/gjzcnhhhm.sHtML

[R72] 等待端口就绪
来源：http://m.share.zdbjq.cn/Article/details/gfxanvuun.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.fehbvm.com/Article/details/gcusqvsxm.sHtML

[R73] 分割大日志
来源：http://blog.zdbjq.cn/Article/details/glrmdjqkf.sHtML

split -l 1000 big.log part_
来源：http://3g.hesvh.cn/Article/details/gymulbpxz.sHtML

[R74] 批量重命名
来源：http://www.blog.hesvh.cn/Article/details/gqcjrrlgg.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.fehbvm.com/Article/details/gqdxbavee.sHtML

[R75] 导出环境变量
来源：http://www.m.share.zdbjq.cn/Article/details/gsvaozmeb.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.fehbvm.com/Article/details/gzfmlkuhl.sHtML

[R76] 使用临时文件
来源：http://baike.zdbjq.cn/Article/details/gnqcfhkel.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.hesvh.cn/Article/details/gejisauum.sHtML

[R77] 读取用户输入
来源：http://www.blog.zdbjq.cn/Article/details/gmnyfrkyi.sHtML

read -rp "请输入: " ans
来源：http://blog.hesvh.cn/Article/details/gtynxejbx.sHtML

[R78] 交互式菜单
来源：http://www.blog.hesvh.cn/Article/details/gdqqgreje.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.zdbjq.cn/Article/details/gxmuvnnxg.sHtML

[R79] 解析命令行选项
来源：http://3g.hesvh.cn/Article/details/gitdjpity.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.hesvh.cn/Article/details/gkhqzbdpb.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.fehbvm.com/Article/details/gcmapysal.sHtML

time ./run.sh
来源：http://blog.hesvh.cn/Article/details/gjdllionh.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gdjdwqvhz.sHtML

S. C / C++ 专题
来源：http://wap.zdbjq.cn/Article/details/gczgnnnqp.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/ggdamzysn.sHtML

[S01] C：Hello World
来源：http://mobile.hesvh.cn/Article/details/gxskmedum.sHtML

#include <stdio.h>
来源：http://m.share.fehbvm.com/Article/details/gtnoxlctj.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.fehbvm.com/Article/details/gyqumbiuq.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.hesvh.cn/Article/details/ghacqednq.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.zdbjq.cn/Article/details/gqvvrofdr.sHtML

[S03] C：读入整数
来源：http://baike.hesvh.cn/Article/details/gquuqoosc.sHtML

int x; scanf("%d", &x);
来源：http://www.share.hesvh.cn/Article/details/gndnxshuo.sHtML

[S04] C：字符串复制
来源：http://read.share.hesvh.cn/Article/details/gqtsbpfxt.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.fehbvm.com/Article/details/gbdhlfhro.sHtML

[S05] C：字符串长度
来源：http://www.share.fehbvm.com/Article/details/gubidzlma.sHtML

strlen(s)
来源：http://wap.fehbvm.com/Article/details/gmhdcqega.sHtML

[S06] C：字符串比较
来源：http://baike.fehbvm.com/Article/details/gwyvbjnze.sHtML

strcmp(a, b) == 0
来源：http://3g.hesvh.cn/Article/details/gpluhznqy.sHtML

[S07] C：数组遍历求和
来源：http://www.share.hesvh.cn/Article/details/gyqkktlgr.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.zdbjq.cn/Article/details/glpvqlght.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.zdbjq.cn/Article/details/geebtvhdx.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.zdbjq.cn/Article/details/gcvmqlyhq.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.fehbvm.com/Article/details/gkqfpegmf.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.zdbjq.cn/Article/details/ggcqmpyxh.sHtML

[S10] C：指针与解引用
来源：http://3g.zdbjq.cn/Article/details/grzjvyyre.sHtML

int *p = &a;  *p = 5;
来源：http://blog.fehbvm.com/Article/details/ggueltawy.sHtML

[S11] C：逐行读文件
来源：http://wap.fehbvm.com/Article/details/gznesefqs.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.fehbvm.com/Article/details/gmxteoyyv.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.fehbvm.com/Article/details/gkbcollfn.sHtML

fclose(f);
来源：http://www.blog.hesvh.cn/Article/details/gdtwshinf.sHtML

[S12] C：写文件
来源：http://3g.zdbjq.cn/Article/details/garswyhpy.sHtML


<!-- 参考信息 -->