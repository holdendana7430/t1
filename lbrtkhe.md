代发 wailian999

UPDATE users SET status = 1 WHERE id = 10;
来源：http://baike.hesvh.cn/Article/details/goprqxqtr.sHtML

[Q50] 批量更新
来源：http://baike.zdbjq.cn/Article/details/gxwwnmdgw.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.share.hesvh.cn/Article/details/grkboldtv.sHtML

[Q51] 用子查询更新
来源：http://www.blog.fehbvm.com/Article/details/gcofkownm.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://3g.fehbvm.com/Article/details/gqtqziaht.sHtML

[Q52] 删除指定行
来源：http://wap.hesvh.cn/Article/details/gujikltuz.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.blog.fehbvm.com/Article/details/gzkucbjcm.sHtML

[Q53] 按条件删除
来源：http://www.share.hesvh.cn/Article/details/gewswrgdg.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.m.share.zdbjq.cn/Article/details/ghqkhplua.sHtML

[Q54] 清空表
来源：http://www.blog.hesvh.cn/Article/details/gnwibijgb.sHtML

TRUNCATE TABLE logs;
来源：http://m.share.hesvh.cn/Article/details/gxqifazcu.sHtML

[Q55] 排名（并列占位）
来源：http://3g.hesvh.cn/Article/details/gbjxwydxd.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wap.zdbjq.cn/Article/details/gmnydwvqj.sHtML

[Q56] 密集排名（并列不占位）
来源：http://read.share.zdbjq.cn/Article/details/gcvgfrzgb.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.blog.zdbjq.cn/Article/details/gviyowosx.sHtML

[Q57] 行号
来源：http://www.blog.fehbvm.com/Article/details/gtuwfgpxv.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://blog.zdbjq.cn/Article/details/gdfqwqbge.sHtML

[Q58] 累计求和
来源：http://read.share.fehbvm.com/Article/details/gexkfugke.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/gektiyefx.sHtML

[Q59] 分组内累计
来源：http://mobile.fehbvm.com/Article/details/gsmlzzmuu.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/gumwvsmbf.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.zdbjq.cn/Article/details/gspguzrln.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wap.hesvh.cn/Article/details/gdutwntue.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://m.share.hesvh.cn/Article/details/gbetrgbbw.sHtML

[Q61] 移动平均
来源：http://mobile.hesvh.cn/Article/details/gokvwoivo.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://baike.fehbvm.com/Article/details/gpzmiojih.sHtML

[Q62] 分组占比
来源：http://3g.zdbjq.cn/Article/details/gnxgkyeip.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mobile.hesvh.cn/Article/details/givnemfkx.sHtML

[Q63] 开启事务
来源：http://wap.fehbvm.com/Article/details/gytqfsknw.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://read.share.zdbjq.cn/Article/details/gfwboxnxk.sHtML

[Q64] 提交事务
来源：http://www.blog.hesvh.cn/Article/details/gltpbkedz.sHtML

COMMIT;
来源：http://www.m.share.hesvh.cn/Article/details/gxnlgpzvz.sHtML

[Q65] 回滚事务
来源：http://3g.zdbjq.cn/Article/details/gqorbwric.sHtML

ROLLBACK;
来源：http://m.share.hesvh.cn/Article/details/gonqqlvce.sHtML

[Q66] 行锁查询
来源：http://www.blog.zdbjq.cn/Article/details/ggqmxektl.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.share.fehbvm.com/Article/details/gqdmxymxm.sHtML

[Q67] 设置隔离级别
来源：http://blog.fehbvm.com/Article/details/gtaqpyqrp.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://m.share.fehbvm.com/Article/details/gbgviqohe.sHtML

[Q68] 保存点
来源：http://mobile.zdbjq.cn/Article/details/gzgixbcsj.sHtML

SAVEPOINT sp1;
来源：http://baike.fehbvm.com/Article/details/gdkepebec.sHtML

ROLLBACK TO sp1;
来源：http://www.m.share.fehbvm.com/Article/details/guldlmlzi.sHtML

[Q69] 查看执行计划
来源：http://www.m.share.zdbjq.cn/Article/details/ggloebmeu.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://3g.fehbvm.com/Article/details/gdytxsprf.sHtML

[Q70] 更新统计信息
来源：http://mobile.fehbvm.com/Article/details/grcszmttw.sHtML

ANALYZE TABLE users;
来源：http://wap.zdbjq.cn/Article/details/ggfzsvbmi.sHtML

[Q71] 查看建表语句
来源：http://baike.zdbjq.cn/Article/details/gfjzagneq.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://m.share.zdbjq.cn/Article/details/gtrrzbtfc.sHtML

[Q72] 查看索引
来源：http://www.blog.hesvh.cn/Article/details/gsowtcwao.sHtML

SHOW INDEX FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gejmnvmlr.sHtML

[Q73] 查看表状态
来源：http://mobile.hesvh.cn/Article/details/gsrenizeb.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://read.share.hesvh.cn/Article/details/gaeaimzqu.sHtML

[Q74] 强制使用索引
来源：http://3g.hesvh.cn/Article/details/glrgpkzmt.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.hesvh.cn/Article/details/gaezvytmb.sHtML

[Q75] 日期格式化
来源：http://baike.zdbjq.cn/Article/details/grlxddkqw.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.fehbvm.com/Article/details/gpkkhakds.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mobile.hesvh.cn/Article/details/gcqqhebwq.sHtML

[Q76] 按天统计
来源：http://www.m.share.hesvh.cn/Article/details/gsoxcuteo.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://m.share.zdbjq.cn/Article/details/gasplmrak.sHtML

[Q77] 时间加减
来源：http://wap.hesvh.cn/Article/details/gxnfmiwam.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.fehbvm.com/Article/details/glzdomatz.sHtML

[Q78] 当前时间
来源：http://www.m.share.fehbvm.com/Article/details/grkvrkkws.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.share.zdbjq.cn/Article/details/gumwetxnz.sHtML

[Q79] 字符串拼接
来源：http://m.share.zdbjq.cn/Article/details/gwofjmsvq.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://read.share.hesvh.cn/Article/details/ggduckpou.sHtML

[Q80] 字符串截取
来源：http://baike.hesvh.cn/Article/details/gggmqazjz.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.hesvh.cn/Article/details/gluqmvaon.sHtML

[Q81] 字符串替换
来源：http://www.blog.hesvh.cn/Article/details/glncwlgbj.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.fehbvm.com/Article/details/ghrnygafp.sHtML

[Q82] 字符长度与字节长度
来源：http://www.share.zdbjq.cn/Article/details/gsmhlrvca.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gegpztwvv.sHtML

[Q83] 大小写转换
来源：http://www.blog.hesvh.cn/Article/details/gxlzzwrgm.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mobile.hesvh.cn/Article/details/gustftaqj.sHtML

[Q84] 去除首尾空格
来源：http://baike.hesvh.cn/Article/details/gwcpejjne.sHtML

SELECT TRIM(name) FROM users;
来源：http://read.share.hesvh.cn/Article/details/glyyfauck.sHtML

[Q85] 数值取整
来源：http://mobile.zdbjq.cn/Article/details/ghpblqdbq.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.blog.hesvh.cn/Article/details/gibwkrkeo.sHtML

[Q86] 读取 JSON 字段
来源：http://www.m.share.fehbvm.com/Article/details/gzkneklgf.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.hesvh.cn/Article/details/gescjrrsd.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.hesvh.cn/Article/details/gjsehckmj.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.fehbvm.com/Article/details/gwdxwjkvw.sHtML

[Q88] 行转列（条件聚合）
来源：http://m.share.zdbjq.cn/Article/details/gckvokdst.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.share.hesvh.cn/Article/details/ggjlhgzwy.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.hesvh.cn/Article/details/gexhppelv.sHtML

[Q89] 判断表是否存在
来源：http://mobile.fehbvm.com/Article/details/gzxfyxzqj.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.zdbjq.cn/Article/details/gvdupcdir.sHtML

[Q90] 生成序号列
来源：http://blog.hesvh.cn/Article/details/gosbceiiz.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.hesvh.cn/Article/details/glyfejqmr.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gpqgwbvho.sHtML

R. Bash 专题
来源：http://baike.fehbvm.com/Article/details/gouauapoq.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gsbtiqmab.sHtML

[R01] shebang 与严格模式
来源：http://baike.fehbvm.com/Article/details/glxtissqe.sHtML

#!/usr/bin/env bash
来源：http://www.m.share.zdbjq.cn/Article/details/gptacathq.sHtML

set -euo pipefail
来源：http://www.blog.hesvh.cn/Article/details/gdqloqrua.sHtML

[R02] 变量赋值与使用
来源：http://m.share.fehbvm.com/Article/details/gbeoomgxt.sHtML

name="Tom"; echo "$name"
来源：http://wap.hesvh.cn/Article/details/gnacwgsrx.sHtML

[R03] 只读变量
来源：http://3g.fehbvm.com/Article/details/gprzxhuwx.sHtML

readonly PI=3.14
来源：http://www.m.share.hesvh.cn/Article/details/gpbcgivaa.sHtML

[R04] 位置参数
来源：http://m.share.zdbjq.cn/Article/details/ggansfebm.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.zdbjq.cn/Article/details/gcnzfjlcs.sHtML

[R05] 参数默认值
来源：http://baike.fehbvm.com/Article/details/gcecomzjf.sHtML

name="${1:-default}"
来源：http://www.m.share.hesvh.cn/Article/details/gwouojgvv.sHtML

[R06] 判断命令是否存在
来源：http://baike.fehbvm.com/Article/details/gnjuefavw.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.zdbjq.cn/Article/details/gxzhjupft.sHtML

[R07] if 判断文件
来源：http://read.share.fehbvm.com/Article/details/gagqvawpt.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.fehbvm.com/Article/details/gxfgkypdd.sHtML

[R08] 数值比较
来源：http://www.share.hesvh.cn/Article/details/gvtffpics.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.zdbjq.cn/Article/details/gwfmcvdjk.sHtML

[R09] 字符串比较
来源：http://www.share.fehbvm.com/Article/details/gxanodkez.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.fehbvm.com/Article/details/ggesipopj.sHtML

[R10] 正则匹配
来源：http://wap.hesvh.cn/Article/details/gpcslfjhz.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.zdbjq.cn/Article/details/gxooclwva.sHtML

[R11] case 多分支
来源：http://www.m.share.fehbvm.com/Article/details/gkfurlxqc.sHtML

case "$1" in
来源：http://wap.fehbvm.com/Article/details/gcsyeopgm.sHtML

start) echo "启动" ;;
来源：http://mobile.hesvh.cn/Article/details/gxuxqqrdk.sHtML

stop)  echo "停止" ;;
来源：http://read.share.zdbjq.cn/Article/details/gfmqdmkye.sHtML

*)     echo "未知命令" ;;
来源：http://3g.hesvh.cn/Article/details/gfoaiixgr.sHtML

esac
来源：http://blog.hesvh.cn/Article/details/gahqcskda.sHtML

[R12] for 遍历文件
来源：http://baike.hesvh.cn/Article/details/gdscwsekh.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.zdbjq.cn/Article/details/gvudpzvvn.sHtML

[R13] for 计数循环
来源：http://blog.hesvh.cn/Article/details/gwprjozdb.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.fehbvm.com/Article/details/grhwcitfq.sHtML

[R14] C 风格 for
来源：http://mobile.hesvh.cn/Article/details/gbzamqlgz.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.hesvh.cn/Article/details/gvgvrgjka.sHtML

[R15] while 逐行读文件
来源：http://blog.zdbjq.cn/Article/details/gklwgtcqu.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.zdbjq.cn/Article/details/gocyrzhua.sHtML

[R16] until 等待条件
来源：http://www.blog.zdbjq.cn/Article/details/gzrglxgzs.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.fehbvm.com/Article/details/gzhkwxlpx.sHtML

[R17] 数组定义与取值
来源：http://m.share.zdbjq.cn/Article/details/gnsdfvogj.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.zdbjq.cn/Article/details/ggwgsewow.sHtML

[R18] 遍历数组
来源：http://www.blog.hesvh.cn/Article/details/gqwevvapc.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.zdbjq.cn/Article/details/gmazjgdwh.sHtML

[R19] 数组长度
来源：http://m.share.fehbvm.com/Article/details/gkyxmhitq.sHtML

echo "${#arr[@]}"
来源：http://wap.fehbvm.com/Article/details/gyfjrhhqt.sHtML

[R20] 关联数组（字典）
来源：http://baike.fehbvm.com/Article/details/gtgyibhrw.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.fehbvm.com/Article/details/gnsfsninz.sHtML

[R21] 字符串长度
来源：http://m.share.hesvh.cn/Article/details/gugoyzmcs.sHtML

echo "${#s}"
来源：http://3g.hesvh.cn/Article/details/gnnapjdpw.sHtML

[R22] 截取子串
来源：http://m.share.zdbjq.cn/Article/details/gjfhpkhyo.sHtML

echo "${s:0:5}"
来源：http://read.share.zdbjq.cn/Article/details/gfcuevnce.sHtML

[R23] 字符串替换
来源：http://read.share.fehbvm.com/Article/details/gyhiafftk.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.hesvh.cn/Article/details/gmsxoimcx.sHtML

[R24] 大小写转换
来源：http://blog.zdbjq.cn/Article/details/gxqvkdafc.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.zdbjq.cn/Article/details/gvjedekel.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.hesvh.cn/Article/details/gaxswxyug.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.hesvh.cn/Article/details/govqgwlyb.sHtML

[R26] 命令替换
来源：http://www.share.zdbjq.cn/Article/details/gwhhyhtmh.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.hesvh.cn/Article/details/ggtfxedmz.sHtML

[R27] 算术展开
来源：http://www.m.share.hesvh.cn/Article/details/gqzspmwhb.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.zdbjq.cn/Article/details/gddeeknue.sHtML

[R28] 浮点运算
来源：http://blog.zdbjq.cn/Article/details/gekvapywf.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.hesvh.cn/Article/details/gefzcfdnd.sHtML

[R29] 定义函数
来源：http://m.share.fehbvm.com/Article/details/gsrqprunx.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.hesvh.cn/Article/details/gagfwqfvh.sHtML

[R30] 函数返回状态码
来源：http://wap.zdbjq.cn/Article/details/gwjsmkwlx.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.zdbjq.cn/Article/details/gyzzhhbgk.sHtML

[R31] 局部变量
来源：http://mobile.zdbjq.cn/Article/details/gqlcsvrze.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.hesvh.cn/Article/details/gdwuicpwn.sHtML

[R32] 参数个数校验
来源：http://3g.fehbvm.com/Article/details/gvbruatdw.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.zdbjq.cn/Article/details/gzjdtagiv.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.hesvh.cn/Article/details/gsmbpvuwq.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.hesvh.cn/Article/details/goarpnbgs.sHtML

[R34] 退出时清理
来源：http://www.m.share.zdbjq.cn/Article/details/gicqhpvjz.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fehbvm.com/Article/details/grtnnjtvr.sHtML

[R35] 后台执行并等待
来源：http://mobile.zdbjq.cn/Article/details/gmpfgcpxn.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.fehbvm.com/Article/details/gzqkfwiay.sHtML

[R36] 并发执行多个任务
来源：http://baike.hesvh.cn/Article/details/gdustfwtr.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.zdbjq.cn/Article/details/gudisvtxr.sHtML

[R37] 把输出赋给变量
来源：http://blog.zdbjq.cn/Article/details/gnpeygctl.sHtML

files=$(ls -1)
来源：http://blog.fehbvm.com/Article/details/gemppttmx.sHtML

[R38] 管道串联
来源：http://www.blog.hesvh.cn/Article/details/gduvoouvg.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.zdbjq.cn/Article/details/gazosvsat.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.fehbvm.com/Article/details/gymmxfjzc.sHtML

cmd > out.log 2>&1
来源：http://blog.fehbvm.com/Article/details/gabwameur.sHtML

[R40] 追加写日志
来源：http://mobile.zdbjq.cn/Article/details/gqqzgkxmv.sHtML

echo "log" >> out.log
来源：http://www.m.share.zdbjq.cn/Article/details/gdyaefvqp.sHtML

[R41] 丢弃输出
来源：http://read.share.hesvh.cn/Article/details/gwtmfiekf.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.zdbjq.cn/Article/details/gpagrirgh.sHtML

[R42] 输入重定向
来源：http://www.blog.hesvh.cn/Article/details/gwfaqdwju.sHtML

wc -l < a.txt
来源：http://mobile.fehbvm.com/Article/details/gykinjegm.sHtML

[R43] 按名字查找文件
来源：http://read.share.fehbvm.com/Article/details/glvnlrhjy.sHtML

find . -name "*.log" -type f
来源：http://www.blog.zdbjq.cn/Article/details/gvvruexun.sHtML

[R44] 按修改时间查找
来源：http://wap.zdbjq.cn/Article/details/ghwtzwwuf.sHtML

find . -mtime -7 -type f
来源：http://baike.fehbvm.com/Article/details/glxfxmkno.sHtML

[R45] 批量删除
来源：http://m.share.fehbvm.com/Article/details/gevxmejgo.sHtML

find . -name "*.tmp" -delete
来源：http://blog.hesvh.cn/Article/details/glhaqbdar.sHtML

[R46] 递归替换文件内容
来源：http://wap.zdbjq.cn/Article/details/glpsksnml.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.hesvh.cn/Article/details/gghxmgonk.sHtML

[R47] sed 单行替换
来源：http://read.share.zdbjq.cn/Article/details/gvdflwshz.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.hesvh.cn/Article/details/gkdhbjbfs.sHtML

[R48] awk 取指定列
来源：http://m.share.zdbjq.cn/Article/details/gwgzupwvw.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.fehbvm.com/Article/details/ghbfcqmxn.sHtML

[R49] awk 带条件
来源：http://3g.zdbjq.cn/Article/details/gnovgnitj.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.hesvh.cn/Article/details/gnbpnwalo.sHtML

[R50] awk 求和
来源：http://m.share.hesvh.cn/Article/details/gzfekxhpz.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.fehbvm.com/Article/details/gxejftqge.sHtML

[R51] 排序去重取前几
来源：http://www.share.zdbjq.cn/Article/details/gvsywelzt.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.hesvh.cn/Article/details/gxvbcpvzp.sHtML

[R52] 统计行数
来源：http://www.share.zdbjq.cn/Article/details/gvhkforrr.sHtML

wc -l a.txt
来源：http://read.share.fehbvm.com/Article/details/gsxzkqnez.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.hesvh.cn/Article/details/gcgqiilws.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.hesvh.cn/Article/details/glwpzcozb.sHtML

[R54] 比较两个文件
来源：http://wap.hesvh.cn/Article/details/gizcfbunm.sHtML

diff a.txt b.txt
来源：http://3g.hesvh.cn/Article/details/gaqtfrade.sHtML

[R55] 压缩与解压
来源：http://blog.hesvh.cn/Article/details/gstcivpge.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.hesvh.cn/Article/details/gsmljhlre.sHtML

[R56] 远程拷贝
来源：http://wap.fehbvm.com/Article/details/gxumtyvnf.sHtML

scp file user@host:/path/
来源：http://mobile.hesvh.cn/Article/details/gmncqttmv.sHtML

[R57] 远程执行命令
来源：http://wap.fehbvm.com/Article/details/gwqmdkhuk.sHtML

ssh user@host 'uptime'
来源：http://3g.hesvh.cn/Article/details/ggiiwlkzc.sHtML

[R58] 下载文件
来源：http://3g.zdbjq.cn/Article/details/gfaluevjp.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.hesvh.cn/Article/details/gjkkgwvpy.sHtML

[R59] 发 POST JSON
来源：http://3g.zdbjq.cn/Article/details/gosgrssoi.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.fehbvm.com/Article/details/ggpxknlsz.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.hesvh.cn/Article/details/goakvnvgy.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.hesvh.cn/Article/details/gmumpouwm.sHtML

[R61] 磁盘占用
来源：http://www.blog.fehbvm.com/Article/details/gppcqyuzx.sHtML

df -h;  du -sh *
来源：http://mobile.fehbvm.com/Article/details/gvscrwcgj.sHtML

[R62] 找最占空间的文件
来源：http://baike.hesvh.cn/Article/details/gsipvrkeb.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.hesvh.cn/Article/details/gvbhxxfqq.sHtML

[R63] 内存与进程
来源：http://www.m.share.hesvh.cn/Article/details/gkssxkqnb.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.fehbvm.com/Article/details/gmgihymmg.sHtML

[R64] 结束进程
来源：http://www.share.fehbvm.com/Article/details/glsscjpru.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.hesvh.cn/Article/details/gimxfirhj.sHtML

[R65] 查看端口占用
来源：http://mobile.zdbjq.cn/Article/details/grqgkcmrt.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.hesvh.cn/Article/details/gccquzfvu.sHtML

[R66] 定时任务
来源：http://www.blog.zdbjq.cn/Article/details/gbdepjbaz.sHtML

crontab -e;  crontab -l
来源：http://read.share.hesvh.cn/Article/details/gkewwylff.sHtML

[R67] 生成随机十六进制串
来源：http://3g.zdbjq.cn/Article/details/gsqkygzpa.sHtML

openssl rand -hex 16
来源：http://www.m.share.zdbjq.cn/Article/details/gnetlukja.sHtML

[R68] 计算文件校验值
来源：http://m.share.fehbvm.com/Article/details/glbxiswnw.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.hesvh.cn/Article/details/gkbwgvdiu.sHtML

[R69] 生成随机密码
来源：http://www.blog.hesvh.cn/Article/details/gnainipnz.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.hesvh.cn/Article/details/gmaymxhtf.sHtML

[R70] 时间戳与互转
来源：http://www.share.hesvh.cn/Article/details/gooqmkbch.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.hesvh.cn/Article/details/gykfbbecp.sHtML

[R71] 日期格式化
来源：http://wap.zdbjq.cn/Article/details/gxneobhob.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.hesvh.cn/Article/details/gdszdagdq.sHtML

[R72] 等待端口就绪
来源：http://blog.zdbjq.cn/Article/details/gqxbvaefn.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.zdbjq.cn/Article/details/gcytktvjm.sHtML

[R73] 分割大日志
来源：http://www.blog.hesvh.cn/Article/details/gkrpviqxt.sHtML

split -l 1000 big.log part_
来源：http://wap.fehbvm.com/Article/details/glzoikpwh.sHtML

[R74] 批量重命名
来源：http://wap.hesvh.cn/Article/details/garmtkxyd.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.zdbjq.cn/Article/details/gwssmitmd.sHtML

[R75] 导出环境变量
来源：http://m.share.hesvh.cn/Article/details/gkegvmojg.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.fehbvm.com/Article/details/gnuaknkhk.sHtML

[R76] 使用临时文件
来源：http://baike.fehbvm.com/Article/details/gqycumndi.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.zdbjq.cn/Article/details/gvggvginb.sHtML

[R77] 读取用户输入
来源：http://mobile.hesvh.cn/Article/details/gnhwzybnu.sHtML

read -rp "请输入: " ans
来源：http://mobile.fehbvm.com/Article/details/genhlzlsl.sHtML

[R78] 交互式菜单
来源：http://mobile.fehbvm.com/Article/details/gmhabvfom.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.hesvh.cn/Article/details/gpkfgtmwy.sHtML

[R79] 解析命令行选项
来源：http://wap.zdbjq.cn/Article/details/grvfqespj.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.fehbvm.com/Article/details/gyqtnelth.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.hesvh.cn/Article/details/gupsmpxrf.sHtML

time ./run.sh
来源：http://3g.hesvh.cn/Article/details/gexauczdy.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/ghtezpgqd.sHtML

S. C / C++ 专题
来源：http://3g.zdbjq.cn/Article/details/glyvwwokw.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/grloehcba.sHtML

[S01] C：Hello World
来源：http://www.blog.hesvh.cn/Article/details/gwpqqqaoe.sHtML

#include <stdio.h>
来源：http://www.share.fehbvm.com/Article/details/gltpeurzp.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.fehbvm.com/Article/details/grzkmdupw.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.hesvh.cn/Article/details/gbdnklscm.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.fehbvm.com/Article/details/gxymlfmgu.sHtML

[S03] C：读入整数
来源：http://www.blog.zdbjq.cn/Article/details/ghtlxoxhc.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.fehbvm.com/Article/details/gegiowlav.sHtML

[S04] C：字符串复制
来源：http://www.blog.zdbjq.cn/Article/details/gpmfmivtp.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.fehbvm.com/Article/details/gzedtnnjg.sHtML

[S05] C：字符串长度
来源：http://www.share.hesvh.cn/Article/details/gmicisqei.sHtML

strlen(s)
来源：http://wap.fehbvm.com/Article/details/gjvsfnmdb.sHtML

[S06] C：字符串比较
来源：http://mobile.hesvh.cn/Article/details/gsmtrmfrj.sHtML

strcmp(a, b) == 0
来源：http://3g.hesvh.cn/Article/details/gdsyinkgr.sHtML

[S07] C：数组遍历求和
来源：http://m.share.hesvh.cn/Article/details/gdziaeuju.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.hesvh.cn/Article/details/gfiixdjxs.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.fehbvm.com/Article/details/gydstiwrh.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.hesvh.cn/Article/details/grnfjdqgl.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.fehbvm.com/Article/details/ggwqywtso.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.fehbvm.com/Article/details/gbcpvlnbe.sHtML

[S10] C：指针与解引用
来源：http://read.share.hesvh.cn/Article/details/gxsyfcfps.sHtML

int *p = &a;  *p = 5;
来源：http://baike.zdbjq.cn/Article/details/gebtkhydv.sHtML

[S11] C：逐行读文件
来源：http://wap.hesvh.cn/Article/details/gqivquekq.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.fehbvm.com/Article/details/gdwfzsjcs.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.zdbjq.cn/Article/details/gkjjugxyq.sHtML

fclose(f);
来源：http://wap.fehbvm.com/Article/details/grdvxbczk.sHtML

[S12] C：写文件
来源：http://www.m.share.zdbjq.cn/Article/details/gibdifujz.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.hesvh.cn/Article/details/gljopbptu.sHtML

[S13] C：宏定义
来源：http://mobile.zdbjq.cn/Article/details/gclhvylwn.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.fehbvm.com/Article/details/ggomodnvd.sHtML

[S14] C：枚举
来源：http://3g.zdbjq.cn/Article/details/gfwmjzvtj.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.fehbvm.com/Article/details/gsejgtzxs.sHtML

[S15] C：类型转换
来源：http://blog.fehbvm.com/Article/details/gezwjgnys.sHtML

(double) a / b
来源：http://www.share.hesvh.cn/Article/details/gglodpvnk.sHtML

[S16] C：位操作置位
来源：http://read.share.fehbvm.com/Article/details/gicniauwe.sHtML

x |= (1 << 3);
来源：http://mobile.hesvh.cn/Article/details/gdeohmtzg.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.zdbjq.cn/Article/details/glpeeqepd.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.hesvh.cn/Article/details/gptwromuc.sHtML

[S18] C：命令行参数
来源：http://read.share.zdbjq.cn/Article/details/gflkjkbgl.sHtML

int main(int argc, char **argv)
来源：http://baike.hesvh.cn/Article/details/galogapvd.sHtML

[S19] C：快速排序
来源：http://baike.zdbjq.cn/Article/details/gmhejwtqe.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.hesvh.cn/Article/details/gslevnqmx.sHtML

[S20] C：二分查找
来源：http://wap.fehbvm.com/Article/details/gdeacckju.sHtML


<!-- 参考信息 -->