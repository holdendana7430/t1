代发 wailian999

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://baike.fanxiaobao.xyz/Article/details/gvcskdoyu.sHtML

[Q56] 密集排名（并列不占位）
来源：http://3g.fanxiaobao.xyz/Article/details/ggfyscodf.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://3g.fanxiaobao.xyz/Article/details/gsumytaig.sHtML

[Q57] 行号
来源：http://3g.fanxiaobao.xyz/Article/details/gaxslzvoq.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/goonvpsaf.sHtML

[Q58] 累计求和
来源：http://mobile.fanxiaobao.xyz/Article/details/gkcdkisuq.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://baike.fanxiaobao.xyz/Article/details/gwqewedsl.sHtML

[Q59] 分组内累计
来源：http://mobile.fanxiaobao.xyz/Article/details/gqwrrglon.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://m.share.fanxiaobao.xyz/Article/details/gxrptzrqt.sHtML

[Q60] 取上一行 / 下一行
来源：http://mobile.fanxiaobao.xyz/Article/details/ghrdecksc.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://m.share.fanxiaobao.xyz/Article/details/gpirislza.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://m.share.fanxiaobao.xyz/Article/details/guiobntya.sHtML

[Q61] 移动平均
来源：http://mobile.fanxiaobao.xyz/Article/details/gobulpwca.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://3g.fanxiaobao.xyz/Article/details/gpwqcmvey.sHtML

[Q62] 分组占比
来源：http://www.share.fanxiaobao.xyz/Article/details/gsolbcjcq.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.fanxiaobao.xyz/Article/details/gzdodtjtf.sHtML

[Q63] 开启事务
来源：http://mobile.fanxiaobao.xyz/Article/details/gmkxpmuqr.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwgarrdvd.sHtML

[Q64] 提交事务
来源：http://3g.fanxiaobao.xyz/Article/details/gwzasosxo.sHtML

COMMIT;
来源：http://read.share.fanxiaobao.xyz/Article/details/graznifqw.sHtML

[Q65] 回滚事务
来源：http://mobile.fanxiaobao.xyz/Article/details/gnivrnipq.sHtML

ROLLBACK;
来源：http://www.share.fanxiaobao.xyz/Article/details/gdqmkkuyh.sHtML

[Q66] 行锁查询
来源：http://blog.fanxiaobao.xyz/Article/details/gxvyvoepx.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gleuglgem.sHtML

[Q67] 设置隔离级别
来源：http://wap.fanxiaobao.xyz/Article/details/gimjsplgd.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://baike.fanxiaobao.xyz/Article/details/grqhoccex.sHtML

[Q68] 保存点
来源：http://3g.fanxiaobao.xyz/Article/details/gcpcopieo.sHtML

SAVEPOINT sp1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gkuduprrl.sHtML

ROLLBACK TO sp1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyxupafhz.sHtML

[Q69] 查看执行计划
来源：http://mobile.fanxiaobao.xyz/Article/details/griwstvkq.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.fanxiaobao.xyz/Article/details/guzqicswv.sHtML

[Q70] 更新统计信息
来源：http://read.share.fanxiaobao.xyz/Article/details/gxmigftwm.sHtML

ANALYZE TABLE users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcmfjvypg.sHtML

[Q71] 查看建表语句
来源：http://read.share.fanxiaobao.xyz/Article/details/gybbmmryh.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.fanxiaobao.xyz/Article/details/gjzlpvkrb.sHtML

[Q72] 查看索引
来源：http://3g.fanxiaobao.xyz/Article/details/gyfgxyzrh.sHtML

SHOW INDEX FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gmwsdouxv.sHtML

[Q73] 查看表状态
来源：http://3g.fanxiaobao.xyz/Article/details/gkpgpbxlc.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://blog.fanxiaobao.xyz/Article/details/gpycgoois.sHtML

[Q74] 强制使用索引
来源：http://mobile.fanxiaobao.xyz/Article/details/givhuzolv.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://blog.fanxiaobao.xyz/Article/details/geuggjiby.sHtML

[Q75] 日期格式化
来源：http://baike.fanxiaobao.xyz/Article/details/gzpwnrftg.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://blog.fanxiaobao.xyz/Article/details/grhthtnoj.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.fanxiaobao.xyz/Article/details/gnkyrehlk.sHtML

[Q76] 按天统计
来源：http://baike.fanxiaobao.xyz/Article/details/gddvfohnw.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.fanxiaobao.xyz/Article/details/gvachljuf.sHtML

[Q77] 时间加减
来源：http://baike.fanxiaobao.xyz/Article/details/gggsemjzj.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://m.share.fanxiaobao.xyz/Article/details/gmvniepgx.sHtML

[Q78] 当前时间
来源：http://baike.fanxiaobao.xyz/Article/details/gtrcrcbmo.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://blog.fanxiaobao.xyz/Article/details/gdhplgejj.sHtML

[Q79] 字符串拼接
来源：http://baike.fanxiaobao.xyz/Article/details/gfzfrkgln.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.fanxiaobao.xyz/Article/details/gafhryikl.sHtML

[Q80] 字符串截取
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfuhrktjq.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gajjrkyrk.sHtML

[Q81] 字符串替换
来源：http://blog.fanxiaobao.xyz/Article/details/grhrbvryt.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gtfrfkjkq.sHtML

[Q82] 字符长度与字节长度
来源：http://m.share.fanxiaobao.xyz/Article/details/gdcpfawbj.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gpkvakycs.sHtML

[Q83] 大小写转换
来源：http://www.share.fanxiaobao.xyz/Article/details/ggscxymxy.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqyqzwrfs.sHtML

[Q84] 去除首尾空格
来源：http://wap.fanxiaobao.xyz/Article/details/gsylxkbvl.sHtML

SELECT TRIM(name) FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gjjgryxkk.sHtML

[Q85] 数值取整
来源：http://3g.fanxiaobao.xyz/Article/details/gzrrltkbv.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvrcuaswz.sHtML

[Q86] 读取 JSON 字段
来源：http://mobile.fanxiaobao.xyz/Article/details/gxnlsidra.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.fanxiaobao.xyz/Article/details/goqxpohya.sHtML

[Q87] JSON 字段做条件
来源：http://baike.fanxiaobao.xyz/Article/details/grzkpmaed.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gakptqyfe.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.fanxiaobao.xyz/Article/details/gykpatjec.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.share.fanxiaobao.xyz/Article/details/gtfxnhssn.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gkojcwcwf.sHtML

[Q89] 判断表是否存在
来源：http://www.share.fanxiaobao.xyz/Article/details/grkznewpe.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.fanxiaobao.xyz/Article/details/gcrklandb.sHtML

[Q90] 生成序号列
来源：http://blog.fanxiaobao.xyz/Article/details/gttkjedpw.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://baike.fanxiaobao.xyz/Article/details/gpcpnjxui.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/geqksyqph.sHtML

R. Bash 专题
来源：http://mobile.fanxiaobao.xyz/Article/details/grzikgbld.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gvjghyazf.sHtML

[R01] shebang 与严格模式
来源：http://baike.fanxiaobao.xyz/Article/details/ghaipnzqg.sHtML

#!/usr/bin/env bash
来源：http://wap.fanxiaobao.xyz/Article/details/ghcmvcudm.sHtML

set -euo pipefail
来源：http://m.share.fanxiaobao.xyz/Article/details/gvjprwrzp.sHtML

[R02] 变量赋值与使用
来源：http://read.share.fanxiaobao.xyz/Article/details/gtnmxqpid.sHtML

name="Tom"; echo "$name"
来源：http://wap.fanxiaobao.xyz/Article/details/gjzdrvbzs.sHtML

[R03] 只读变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gjikbpujk.sHtML

readonly PI=3.14
来源：http://baike.fanxiaobao.xyz/Article/details/gniibiywa.sHtML

[R04] 位置参数
来源：http://mobile.fanxiaobao.xyz/Article/details/goecxejxh.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.fanxiaobao.xyz/Article/details/gmfyanibd.sHtML

[R05] 参数默认值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpdptrbpn.sHtML

name="${1:-default}"
来源：http://read.share.fanxiaobao.xyz/Article/details/glouqobwm.sHtML

[R06] 判断命令是否存在
来源：http://blog.fanxiaobao.xyz/Article/details/gklswxdwf.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.fanxiaobao.xyz/Article/details/gddbqexwp.sHtML

[R07] if 判断文件
来源：http://baike.fanxiaobao.xyz/Article/details/gfyetceyt.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://baike.fanxiaobao.xyz/Article/details/gxyyrrtoa.sHtML

[R08] 数值比较
来源：http://read.share.fanxiaobao.xyz/Article/details/gnlpncjsr.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/gphwfrrjw.sHtML

[R09] 字符串比较
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxpuayxmv.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.fanxiaobao.xyz/Article/details/gliwhzoze.sHtML

[R10] 正则匹配
来源：http://m.share.fanxiaobao.xyz/Article/details/ghzrlksfp.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.fanxiaobao.xyz/Article/details/gajxczwre.sHtML

[R11] case 多分支
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glrvnqkqb.sHtML

case "$1" in
来源：http://www.share.fanxiaobao.xyz/Article/details/gtzkbsgdh.sHtML

start) echo "启动" ;;
来源：http://mobile.fanxiaobao.xyz/Article/details/gnlkscoaf.sHtML

stop)  echo "停止" ;;
来源：http://read.share.fanxiaobao.xyz/Article/details/gfzmomkbs.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.fanxiaobao.xyz/Article/details/ghgefzycp.sHtML

esac
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzsbxicoo.sHtML

[R12] for 遍历文件
来源：http://blog.fanxiaobao.xyz/Article/details/gwcyzrvtw.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gthoqfipx.sHtML

[R13] for 计数循环
来源：http://blog.fanxiaobao.xyz/Article/details/gdyrlgdab.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/garznydsd.sHtML

[R14] C 风格 for
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzdjsbgbi.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.fanxiaobao.xyz/Article/details/gagctssen.sHtML

[R15] while 逐行读文件
来源：http://blog.fanxiaobao.xyz/Article/details/gjfmxnjdy.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gnkkovubh.sHtML

[R16] until 等待条件
来源：http://blog.fanxiaobao.xyz/Article/details/ghcmxscxe.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.fanxiaobao.xyz/Article/details/gyviihvtv.sHtML

[R17] 数组定义与取值
来源：http://3g.fanxiaobao.xyz/Article/details/gyqkntubk.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gltcgcgnx.sHtML

[R18] 遍历数组
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqadxggpq.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gmxlutwcq.sHtML

[R19] 数组长度
来源：http://3g.fanxiaobao.xyz/Article/details/gwbfvgxav.sHtML

echo "${#arr[@]}"
来源：http://baike.fanxiaobao.xyz/Article/details/gmhxyuftr.sHtML

[R20] 关联数组（字典）
来源：http://m.share.fanxiaobao.xyz/Article/details/gzzqfmxfb.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyngzeowm.sHtML

[R21] 字符串长度
来源：http://read.share.fanxiaobao.xyz/Article/details/gapofzskh.sHtML

echo "${#s}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzbmqntee.sHtML

[R22] 截取子串
来源：http://mobile.fanxiaobao.xyz/Article/details/gcirnfnew.sHtML

echo "${s:0:5}"
来源：http://wap.fanxiaobao.xyz/Article/details/geoysxejo.sHtML

[R23] 字符串替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gznzjwwru.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.fanxiaobao.xyz/Article/details/glekktutx.sHtML

[R24] 大小写转换
来源：http://3g.fanxiaobao.xyz/Article/details/gttjffyam.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.fanxiaobao.xyz/Article/details/gaikekauk.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.fanxiaobao.xyz/Article/details/glrmalnhd.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gatlvaqxq.sHtML

[R26] 命令替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gvwievruv.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gloozgeae.sHtML

[R27] 算术展开
来源：http://read.share.fanxiaobao.xyz/Article/details/gbsaspqra.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.fanxiaobao.xyz/Article/details/gthgxgsvy.sHtML

[R28] 浮点运算
来源：http://3g.fanxiaobao.xyz/Article/details/gyerrsbuj.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.fanxiaobao.xyz/Article/details/gbsshhsda.sHtML

[R29] 定义函数
来源：http://blog.fanxiaobao.xyz/Article/details/glkuupqed.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.fanxiaobao.xyz/Article/details/gdvwfofuk.sHtML

[R30] 函数返回状态码
来源：http://baike.fanxiaobao.xyz/Article/details/gwhblvcyj.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.fanxiaobao.xyz/Article/details/gjrdlpzgj.sHtML

[R31] 局部变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnjeqmcri.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.fanxiaobao.xyz/Article/details/girhqwgfq.sHtML

[R32] 参数个数校验
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbgmswazk.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gmqxfjvkb.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.fanxiaobao.xyz/Article/details/gknozntqc.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.fanxiaobao.xyz/Article/details/gzayvupxn.sHtML

[R34] 退出时清理
来源：http://baike.fanxiaobao.xyz/Article/details/gpymhdioi.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fanxiaobao.xyz/Article/details/gfzrxkbkp.sHtML

[R35] 后台执行并等待
来源：http://baike.fanxiaobao.xyz/Article/details/ggnzfqvjt.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.fanxiaobao.xyz/Article/details/gxjfjtufv.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbtmefhmx.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.fanxiaobao.xyz/Article/details/gkjfgqqzj.sHtML

[R37] 把输出赋给变量
来源：http://mobile.fanxiaobao.xyz/Article/details/guamideol.sHtML

files=$(ls -1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gwrlizvzn.sHtML

[R38] 管道串联
来源：http://mobile.fanxiaobao.xyz/Article/details/gfcfyjdpd.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.fanxiaobao.xyz/Article/details/gwndjmowv.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.fanxiaobao.xyz/Article/details/gzyuorgtf.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjkvbyevw.sHtML

[R40] 追加写日志
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdwsammxq.sHtML

echo "log" >> out.log
来源：http://baike.fanxiaobao.xyz/Article/details/gkdscsfob.sHtML

[R41] 丢弃输出
来源：http://blog.fanxiaobao.xyz/Article/details/gdvacpvbx.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.fanxiaobao.xyz/Article/details/gjjlnsoew.sHtML

[R42] 输入重定向
来源：http://read.share.fanxiaobao.xyz/Article/details/givvjbtee.sHtML

wc -l < a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwgotewzp.sHtML

[R43] 按名字查找文件
来源：http://baike.fanxiaobao.xyz/Article/details/geszhbsco.sHtML

find . -name "*.log" -type f
来源：http://mobile.fanxiaobao.xyz/Article/details/gghjcxiyw.sHtML

[R44] 按修改时间查找
来源：http://m.share.fanxiaobao.xyz/Article/details/gxdjmzopf.sHtML

find . -mtime -7 -type f
来源：http://m.share.fanxiaobao.xyz/Article/details/gckzemkjy.sHtML

[R45] 批量删除
来源：http://baike.fanxiaobao.xyz/Article/details/gzfhqhevq.sHtML

find . -name "*.tmp" -delete
来源：http://3g.fanxiaobao.xyz/Article/details/gghzvjnnq.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkulwxcjb.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.fanxiaobao.xyz/Article/details/grnemgbcy.sHtML

[R47] sed 单行替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/giawaioxf.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gxrtgovue.sHtML

[R48] awk 取指定列
来源：http://www.share.fanxiaobao.xyz/Article/details/gndrrkxah.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gozuatcqz.sHtML

[R49] awk 带条件
来源：http://m.share.fanxiaobao.xyz/Article/details/gjsfkivjx.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.fanxiaobao.xyz/Article/details/ggdpukfbq.sHtML

[R50] awk 求和
来源：http://m.share.fanxiaobao.xyz/Article/details/gjiebuifb.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gbbpkrsnt.sHtML

[R51] 排序去重取前几
来源：http://mobile.fanxiaobao.xyz/Article/details/ggqctnwgo.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.fanxiaobao.xyz/Article/details/gvdiopzur.sHtML

[R52] 统计行数
来源：http://read.share.fanxiaobao.xyz/Article/details/gcjlrnacs.sHtML

wc -l a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/ggexjodpk.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.fanxiaobao.xyz/Article/details/gdzoxclbs.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.fanxiaobao.xyz/Article/details/ggncxgpce.sHtML

[R54] 比较两个文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gydavejva.sHtML

diff a.txt b.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gvcoijxod.sHtML

[R55] 压缩与解压
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gisxocwaw.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gziwxewii.sHtML

[R56] 远程拷贝
来源：http://baike.fanxiaobao.xyz/Article/details/gdrabnvse.sHtML

scp file user@host:/path/
来源：http://mobile.fanxiaobao.xyz/Article/details/gmzaebnzu.sHtML

[R57] 远程执行命令
来源：http://3g.fanxiaobao.xyz/Article/details/gwbntngny.sHtML

ssh user@host 'uptime'
来源：http://www.share.fanxiaobao.xyz/Article/details/gwtytugjg.sHtML

[R58] 下载文件
来源：http://m.share.fanxiaobao.xyz/Article/details/giixlnskn.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.fanxiaobao.xyz/Article/details/guontsvpz.sHtML

[R59] 发 POST JSON
来源：http://m.share.fanxiaobao.xyz/Article/details/gwnbyqvju.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.fanxiaobao.xyz/Article/details/gktauxthg.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxiqzjfwk.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.fanxiaobao.xyz/Article/details/gnfudablx.sHtML

[R61] 磁盘占用
来源：http://m.share.fanxiaobao.xyz/Article/details/gpskrmvbn.sHtML

df -h;  du -sh *
来源：http://wap.fanxiaobao.xyz/Article/details/gokozlwwj.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpphuapyk.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.fanxiaobao.xyz/Article/details/gahdzyxzo.sHtML

[R63] 内存与进程
来源：http://read.share.fanxiaobao.xyz/Article/details/gmwqboobn.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.fanxiaobao.xyz/Article/details/gdfrsmnyx.sHtML

[R64] 结束进程
来源：http://wap.fanxiaobao.xyz/Article/details/gifmstpme.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnmblmswl.sHtML

[R65] 查看端口占用
来源：http://www.share.fanxiaobao.xyz/Article/details/genzuclww.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.fanxiaobao.xyz/Article/details/gnvbdqoom.sHtML

[R66] 定时任务
来源：http://wap.fanxiaobao.xyz/Article/details/ggpmkncnv.sHtML

crontab -e;  crontab -l
来源：http://www.share.fanxiaobao.xyz/Article/details/grvhkmuhh.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.fanxiaobao.xyz/Article/details/goqhqbstt.sHtML

openssl rand -hex 16
来源：http://read.share.fanxiaobao.xyz/Article/details/glbntfyoz.sHtML

[R68] 计算文件校验值
来源：http://m.share.fanxiaobao.xyz/Article/details/gbscaypjn.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gbpzttwwo.sHtML

[R69] 生成随机密码
来源：http://mobile.fanxiaobao.xyz/Article/details/gxmkyestu.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.fanxiaobao.xyz/Article/details/gcyrmrskz.sHtML

[R70] 时间戳与互转
来源：http://www.share.fanxiaobao.xyz/Article/details/gqpjrpgvv.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.fanxiaobao.xyz/Article/details/gimcyxrae.sHtML

[R71] 日期格式化
来源：http://blog.fanxiaobao.xyz/Article/details/gbcjbkwrl.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://read.share.fanxiaobao.xyz/Article/details/guuhxdmjr.sHtML

[R72] 等待端口就绪
来源：http://baike.fanxiaobao.xyz/Article/details/gtumvxdpk.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.fanxiaobao.xyz/Article/details/gncsjkpnl.sHtML

[R73] 分割大日志
来源：http://wap.fanxiaobao.xyz/Article/details/glmxrkhvb.sHtML

split -l 1000 big.log part_
来源：http://wap.fanxiaobao.xyz/Article/details/gzkzwgmcg.sHtML

[R74] 批量重命名
来源：http://www.share.fanxiaobao.xyz/Article/details/gccpbhyym.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gojlmrask.sHtML

[R75] 导出环境变量
来源：http://blog.fanxiaobao.xyz/Article/details/gupylgoke.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.fanxiaobao.xyz/Article/details/gnaiiqbfm.sHtML

[R76] 使用临时文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gmxwagldi.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.fanxiaobao.xyz/Article/details/gaebdnfwm.sHtML

[R77] 读取用户输入
来源：http://www.share.fanxiaobao.xyz/Article/details/gzpvutuos.sHtML

read -rp "请输入: " ans
来源：http://mobile.fanxiaobao.xyz/Article/details/gijmibdzl.sHtML

[R78] 交互式菜单
来源：http://blog.fanxiaobao.xyz/Article/details/gnbsoxyyj.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.fanxiaobao.xyz/Article/details/gzfnlyjhv.sHtML

[R79] 解析命令行选项
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkkrltkcb.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.fanxiaobao.xyz/Article/details/gjurtwpkb.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.fanxiaobao.xyz/Article/details/gyjkblbnw.sHtML

time ./run.sh
来源：http://3g.fanxiaobao.xyz/Article/details/gmenjrnyl.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gxnlhcbak.sHtML

S. C / C++ 专题
来源：http://baike.fanxiaobao.xyz/Article/details/gtgdkmkut.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gonpwsdpt.sHtML

[S01] C：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnlrgwsvn.sHtML

#include <stdio.h>
来源：http://www.share.fanxiaobao.xyz/Article/details/gkqagmivy.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.fanxiaobao.xyz/Article/details/ghjazpjdn.sHtML

[S02] C：变量与格式化输出
来源：http://3g.fanxiaobao.xyz/Article/details/gvjlotvxh.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.fanxiaobao.xyz/Article/details/glcablcoh.sHtML

[S03] C：读入整数
来源：http://www.share.fanxiaobao.xyz/Article/details/gplterrba.sHtML

int x; scanf("%d", &x);
来源：http://blog.fanxiaobao.xyz/Article/details/gqepjqfho.sHtML

[S04] C：字符串复制
来源：http://wap.fanxiaobao.xyz/Article/details/gguwkvxck.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.fanxiaobao.xyz/Article/details/gsslacnyv.sHtML

[S05] C：字符串长度
来源：http://read.share.fanxiaobao.xyz/Article/details/garewwxzi.sHtML

strlen(s)
来源：http://www.share.fanxiaobao.xyz/Article/details/gerwbjpdy.sHtML

[S06] C：字符串比较
来源：http://wap.fanxiaobao.xyz/Article/details/gdsycasom.sHtML

strcmp(a, b) == 0
来源：http://3g.fanxiaobao.xyz/Article/details/gndvdsmfl.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpbdsiyxq.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.fanxiaobao.xyz/Article/details/ghaczupxj.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkmhpxhda.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.fanxiaobao.xyz/Article/details/gkhtfgmya.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.fanxiaobao.xyz/Article/details/gkcxjdsnq.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.fanxiaobao.xyz/Article/details/grixsnykt.sHtML

[S10] C：指针与解引用
来源：http://mobile.fanxiaobao.xyz/Article/details/gorxzfpmt.sHtML

int *p = &a;  *p = 5;
来源：http://blog.fanxiaobao.xyz/Article/details/gmqehkzkp.sHtML

[S11] C：逐行读文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gktsejyov.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.fanxiaobao.xyz/Article/details/giiqusska.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.fanxiaobao.xyz/Article/details/gfdiyoras.sHtML

fclose(f);
来源：http://3g.fanxiaobao.xyz/Article/details/gszeymrnv.sHtML

[S12] C：写文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gtzyvmywt.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gphovlwjv.sHtML

[S13] C：宏定义
来源：http://baike.fanxiaobao.xyz/Article/details/gavkfinrg.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.fanxiaobao.xyz/Article/details/gjlvxddki.sHtML

[S14] C：枚举
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtwqdutpt.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.fanxiaobao.xyz/Article/details/gqsktvqvb.sHtML

[S15] C：类型转换
来源：http://3g.fanxiaobao.xyz/Article/details/gjowligzj.sHtML

(double) a / b
来源：http://wap.fanxiaobao.xyz/Article/details/gupmamldp.sHtML

[S16] C：位操作置位
来源：http://baike.fanxiaobao.xyz/Article/details/glruyzbkt.sHtML

x |= (1 << 3);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glopqkoas.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmqovleoy.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.fanxiaobao.xyz/Article/details/gtoeyouad.sHtML

[S18] C：命令行参数
来源：http://read.share.fanxiaobao.xyz/Article/details/gqwcnlbji.sHtML

int main(int argc, char **argv)
来源：http://baike.fanxiaobao.xyz/Article/details/gvohcwtel.sHtML

[S19] C：快速排序
来源：http://mobile.fanxiaobao.xyz/Article/details/gtfkqiwtb.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.fanxiaobao.xyz/Article/details/gphmditiv.sHtML

[S20] C：二分查找
来源：http://www.share.fanxiaobao.xyz/Article/details/gyssoucic.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.fanxiaobao.xyz/Article/details/getonjwkp.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzdnbzahx.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghoyxfuic.sHtML

[S22] C：字符串转数字
来源：http://blog.fanxiaobao.xyz/Article/details/ggmlfqawc.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.fanxiaobao.xyz/Article/details/gqqqmauyl.sHtML

[S23] C：随机数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzroximvu.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.fanxiaobao.xyz/Article/details/ggxkfqwuv.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsittjkkb.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.fanxiaobao.xyz/Article/details/gkssoqcdt.sHtML

[S25] C：内存拷贝
来源：http://3g.fanxiaobao.xyz/Article/details/gmwogwnao.sHtML

memcpy(dst, src, n);
来源：http://baike.fanxiaobao.xyz/Article/details/ggewqgrpl.sHtML

[S26] C：内存清零
来源：http://www.share.fanxiaobao.xyz/Article/details/ghrferwkm.sHtML


<!-- 参考信息 -->