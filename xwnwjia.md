代发 wailian999

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://m.share.fanxiaobao.xyz/Article/details/gxnclhrhs.sHtML

[Q54] 清空表
来源：http://m.share.fanxiaobao.xyz/Article/details/gijwoajst.sHtML

TRUNCATE TABLE logs;
来源：http://www.share.fanxiaobao.xyz/Article/details/gxmxqyshi.sHtML

[Q55] 排名（并列占位）
来源：http://3g.fanxiaobao.xyz/Article/details/gabjgqysg.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://blog.fanxiaobao.xyz/Article/details/gackocwjp.sHtML

[Q56] 密集排名（并列不占位）
来源：http://m.share.fanxiaobao.xyz/Article/details/gkdvcixcu.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdsjykbob.sHtML

[Q57] 行号
来源：http://mobile.fanxiaobao.xyz/Article/details/gsjnivioa.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gdksrvrmh.sHtML

[Q58] 累计求和
来源：http://3g.fanxiaobao.xyz/Article/details/guqwmursn.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://baike.fanxiaobao.xyz/Article/details/gxwpvjfkr.sHtML

[Q59] 分组内累计
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfgzbeaoq.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://blog.fanxiaobao.xyz/Article/details/gvtzcacth.sHtML

[Q60] 取上一行 / 下一行
来源：http://wap.fanxiaobao.xyz/Article/details/gkktrvocq.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://3g.fanxiaobao.xyz/Article/details/ggvyymduf.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.share.fanxiaobao.xyz/Article/details/gprgirxxj.sHtML

[Q61] 移动平均
来源：http://blog.fanxiaobao.xyz/Article/details/glcufrovy.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://baike.fanxiaobao.xyz/Article/details/gpcrojvax.sHtML

[Q62] 分组占比
来源：http://mobile.fanxiaobao.xyz/Article/details/gqiprrcwx.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://3g.fanxiaobao.xyz/Article/details/gvlvensdb.sHtML

[Q63] 开启事务
来源：http://wap.fanxiaobao.xyz/Article/details/guixnajzn.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://baike.fanxiaobao.xyz/Article/details/gfwlgrdgb.sHtML

[Q64] 提交事务
来源：http://baike.fanxiaobao.xyz/Article/details/ggmjhpgay.sHtML

COMMIT;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqitiqjzj.sHtML

[Q65] 回滚事务
来源：http://3g.fanxiaobao.xyz/Article/details/gmryrmzab.sHtML

ROLLBACK;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdhdsyapx.sHtML

[Q66] 行锁查询
来源：http://baike.fanxiaobao.xyz/Article/details/gmqhamqkc.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.fanxiaobao.xyz/Article/details/ghxldduti.sHtML

[Q67] 设置隔离级别
来源：http://m.share.fanxiaobao.xyz/Article/details/ggapgieou.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://read.share.fanxiaobao.xyz/Article/details/gjtoxfmwb.sHtML

[Q68] 保存点
来源：http://wap.fanxiaobao.xyz/Article/details/gowokqisi.sHtML

SAVEPOINT sp1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzmefpmap.sHtML

ROLLBACK TO sp1;
来源：http://3g.fanxiaobao.xyz/Article/details/gzetqoshe.sHtML

[Q69] 查看执行计划
来源：http://www.share.fanxiaobao.xyz/Article/details/gogemrhjf.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.share.fanxiaobao.xyz/Article/details/gpsnqwgjn.sHtML

[Q70] 更新统计信息
来源：http://mobile.fanxiaobao.xyz/Article/details/gshumopnz.sHtML

ANALYZE TABLE users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gtdtwapiq.sHtML

[Q71] 查看建表语句
来源：http://wap.fanxiaobao.xyz/Article/details/gfyoggfpy.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gripteiam.sHtML

[Q72] 查看索引
来源：http://read.share.fanxiaobao.xyz/Article/details/geimtanae.sHtML

SHOW INDEX FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gasviemuy.sHtML

[Q73] 查看表状态
来源：http://wap.fanxiaobao.xyz/Article/details/gqzbzvkke.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.share.fanxiaobao.xyz/Article/details/gkohlyodu.sHtML

[Q74] 强制使用索引
来源：http://wap.fanxiaobao.xyz/Article/details/gefpeybtw.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mobile.fanxiaobao.xyz/Article/details/gkigwzgbo.sHtML

[Q75] 日期格式化
来源：http://3g.fanxiaobao.xyz/Article/details/gvtatsmnw.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wap.fanxiaobao.xyz/Article/details/gccnvveaa.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wap.fanxiaobao.xyz/Article/details/gbbnowgur.sHtML

[Q76] 按天统计
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkwpcshjc.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.blog.fanxiaobao.xyz/Article/details/geqjzeehz.sHtML

[Q77] 时间加减
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gisnspztj.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://3g.fanxiaobao.xyz/Article/details/gjijwkkbt.sHtML

[Q78] 当前时间
来源：http://read.share.fanxiaobao.xyz/Article/details/gnxdxqlul.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.blog.fanxiaobao.xyz/Article/details/grnsfurxe.sHtML

[Q79] 字符串拼接
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaotafqbm.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://baike.fanxiaobao.xyz/Article/details/guqoxogld.sHtML

[Q80] 字符串截取
来源：http://3g.fanxiaobao.xyz/Article/details/gckeyvpvt.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/ghdwaqbey.sHtML

[Q81] 字符串替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbmxddxpr.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gvrbtgodm.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.fanxiaobao.xyz/Article/details/gegierrbf.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gbhzbxoct.sHtML

[Q83] 大小写转换
来源：http://wap.fanxiaobao.xyz/Article/details/govasmkla.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gdyoeiydn.sHtML

[Q84] 去除首尾空格
来源：http://3g.fanxiaobao.xyz/Article/details/gwjecarlu.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gainohydi.sHtML

[Q85] 数值取整
来源：http://3g.fanxiaobao.xyz/Article/details/gmnxocqga.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcvwklirs.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.fanxiaobao.xyz/Article/details/gxexjlgce.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.fanxiaobao.xyz/Article/details/gjpidvzxa.sHtML

[Q87] JSON 字段做条件
来源：http://read.share.fanxiaobao.xyz/Article/details/gjtnfehgq.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.fanxiaobao.xyz/Article/details/gymwdfyez.sHtML

[Q88] 行转列（条件聚合）
来源：http://m.share.fanxiaobao.xyz/Article/details/gfrusukoh.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://read.share.fanxiaobao.xyz/Article/details/gadujtgcr.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gmjxnudoo.sHtML

[Q89] 判断表是否存在
来源：http://m.share.fanxiaobao.xyz/Article/details/gssjwoikj.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.fanxiaobao.xyz/Article/details/grccitxhz.sHtML

[Q90] 生成序号列
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqqgnbyxm.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.fanxiaobao.xyz/Article/details/galzfibhw.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gxudhfpsj.sHtML

R. Bash 专题
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdgtfboyp.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gehttblfs.sHtML

[R01] shebang 与严格模式
来源：http://baike.fanxiaobao.xyz/Article/details/gbfxbaxbg.sHtML

#!/usr/bin/env bash
来源：http://3g.fanxiaobao.xyz/Article/details/gibzaorbg.sHtML

set -euo pipefail
来源：http://blog.fanxiaobao.xyz/Article/details/gxjwmdynp.sHtML

[R02] 变量赋值与使用
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyjwgqznc.sHtML

name="Tom"; echo "$name"
来源：http://blog.fanxiaobao.xyz/Article/details/gckmgbtyr.sHtML

[R03] 只读变量
来源：http://baike.fanxiaobao.xyz/Article/details/gwlmdfehi.sHtML

readonly PI=3.14
来源：http://blog.fanxiaobao.xyz/Article/details/gajbgeirb.sHtML

[R04] 位置参数
来源：http://www.share.fanxiaobao.xyz/Article/details/gzsytkywy.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.fanxiaobao.xyz/Article/details/gqwvqfgwj.sHtML

[R05] 参数默认值
来源：http://baike.fanxiaobao.xyz/Article/details/gcdelbndy.sHtML

name="${1:-default}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gmbrtxuwy.sHtML

[R06] 判断命令是否存在
来源：http://3g.fanxiaobao.xyz/Article/details/gmaepgoqo.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gxedhrgxp.sHtML

[R07] if 判断文件
来源：http://baike.fanxiaobao.xyz/Article/details/gdjibxvyf.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gydyupdfh.sHtML

[R08] 数值比较
来源：http://baike.fanxiaobao.xyz/Article/details/gooejezlb.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjwekfwwb.sHtML

[R09] 字符串比较
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gglgubpgx.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glplmidmk.sHtML

[R10] 正则匹配
来源：http://wap.fanxiaobao.xyz/Article/details/grnhpfxdc.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.fanxiaobao.xyz/Article/details/glzafvzqi.sHtML

[R11] case 多分支
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwwrxscri.sHtML

case "$1" in
来源：http://www.blog.fanxiaobao.xyz/Article/details/grryhfmnm.sHtML

start) echo "启动" ;;
来源：http://www.share.fanxiaobao.xyz/Article/details/guhsxvthr.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gendfvfnv.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.fanxiaobao.xyz/Article/details/gqyizztth.sHtML

esac
来源：http://baike.fanxiaobao.xyz/Article/details/gghlrfjkj.sHtML

[R12] for 遍历文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjsfehzha.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gclnkynam.sHtML

[R13] for 计数循环
来源：http://wap.fanxiaobao.xyz/Article/details/gskscrtps.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.fanxiaobao.xyz/Article/details/gcigpgpdz.sHtML

[R14] C 风格 for
来源：http://read.share.fanxiaobao.xyz/Article/details/glqlwvzno.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gudnqnrqr.sHtML

[R15] while 逐行读文件
来源：http://blog.fanxiaobao.xyz/Article/details/gffaoxxdh.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/giwtnqept.sHtML

[R16] until 等待条件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/govrnlgmo.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gujbrhpvb.sHtML

[R17] 数组定义与取值
来源：http://www.share.fanxiaobao.xyz/Article/details/gvvhtfjli.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gabduhhof.sHtML

[R18] 遍历数组
来源：http://baike.fanxiaobao.xyz/Article/details/gofvvscxi.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/goldevghk.sHtML

[R19] 数组长度
来源：http://www.share.fanxiaobao.xyz/Article/details/gfktpydwj.sHtML

echo "${#arr[@]}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gsyfyykqy.sHtML

[R20] 关联数组（字典）
来源：http://baike.fanxiaobao.xyz/Article/details/gbugjsdxl.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wap.fanxiaobao.xyz/Article/details/guzkfmryh.sHtML

[R21] 字符串长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfcawtcyb.sHtML

echo "${#s}"
来源：http://baike.fanxiaobao.xyz/Article/details/gebsrovrd.sHtML

[R22] 截取子串
来源：http://www.share.fanxiaobao.xyz/Article/details/gnxeitvpr.sHtML

echo "${s:0:5}"
来源：http://3g.fanxiaobao.xyz/Article/details/gsxjdwczp.sHtML

[R23] 字符串替换
来源：http://blog.fanxiaobao.xyz/Article/details/giblrthdx.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.fanxiaobao.xyz/Article/details/gynjlrjpb.sHtML

[R24] 大小写转换
来源：http://wap.fanxiaobao.xyz/Article/details/gkrtvvgbn.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvbfkpusy.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.fanxiaobao.xyz/Article/details/gmbiawsge.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbrnuehkf.sHtML

[R26] 命令替换
来源：http://3g.fanxiaobao.xyz/Article/details/gnqlespez.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjvufrqzz.sHtML

[R27] 算术展开
来源：http://m.share.fanxiaobao.xyz/Article/details/gtggwbsud.sHtML

echo $((1 + 2 * 3))
来源：http://blog.fanxiaobao.xyz/Article/details/gjzzugviy.sHtML

[R28] 浮点运算
来源：http://www.share.fanxiaobao.xyz/Article/details/gcimksicq.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.fanxiaobao.xyz/Article/details/gsojldqxu.sHtML

[R29] 定义函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gshybidth.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.fanxiaobao.xyz/Article/details/ggbcplweq.sHtML

[R30] 函数返回状态码
来源：http://3g.fanxiaobao.xyz/Article/details/gsbmxytbg.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.fanxiaobao.xyz/Article/details/gocevvaop.sHtML

[R31] 局部变量
来源：http://m.share.fanxiaobao.xyz/Article/details/guvuzbhmv.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.fanxiaobao.xyz/Article/details/gmqmecuuz.sHtML

[R32] 参数个数校验
来源：http://baike.fanxiaobao.xyz/Article/details/gxyrmuovn.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.fanxiaobao.xyz/Article/details/gyyhnwhmr.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.fanxiaobao.xyz/Article/details/gnblgasxw.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.fanxiaobao.xyz/Article/details/gkfxxpzzu.sHtML

[R34] 退出时清理
来源：http://3g.fanxiaobao.xyz/Article/details/gfsltbtgt.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.share.fanxiaobao.xyz/Article/details/grtewrmkt.sHtML

[R35] 后台执行并等待
来源：http://blog.fanxiaobao.xyz/Article/details/gefippgfn.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.fanxiaobao.xyz/Article/details/gvognxwwj.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gasuqujir.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.fanxiaobao.xyz/Article/details/ggljqfpjj.sHtML

[R37] 把输出赋给变量
来源：http://wap.fanxiaobao.xyz/Article/details/gniywzesk.sHtML

files=$(ls -1)
来源：http://3g.fanxiaobao.xyz/Article/details/gindbkyky.sHtML

[R38] 管道串联
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gofttowsa.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.fanxiaobao.xyz/Article/details/gfuknrupz.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.fanxiaobao.xyz/Article/details/givurucgw.sHtML

cmd > out.log 2>&1
来源：http://wap.fanxiaobao.xyz/Article/details/gkrjtonyu.sHtML

[R40] 追加写日志
来源：http://3g.fanxiaobao.xyz/Article/details/glsixzfqz.sHtML

echo "log" >> out.log
来源：http://blog.fanxiaobao.xyz/Article/details/gtuywlsbf.sHtML

[R41] 丢弃输出
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbrdyvbjz.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gussfuzyh.sHtML

[R42] 输入重定向
来源：http://www.share.fanxiaobao.xyz/Article/details/gcvwmpohp.sHtML

wc -l < a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gvqpukxbv.sHtML

[R43] 按名字查找文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gjzpwpnxj.sHtML

find . -name "*.log" -type f
来源：http://wap.fanxiaobao.xyz/Article/details/gnmxnrfgd.sHtML

[R44] 按修改时间查找
来源：http://baike.fanxiaobao.xyz/Article/details/gnhlfvidg.sHtML

find . -mtime -7 -type f
来源：http://blog.fanxiaobao.xyz/Article/details/gbhhvggbf.sHtML

[R45] 批量删除
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gymnbgevs.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxzsafodn.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyfexcerd.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.fanxiaobao.xyz/Article/details/gmduteaev.sHtML

[R47] sed 单行替换
来源：http://3g.fanxiaobao.xyz/Article/details/gwotxzxeu.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gowsjxvhj.sHtML

[R48] awk 取指定列
来源：http://read.share.fanxiaobao.xyz/Article/details/gfzbgllep.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gcpuwdvxp.sHtML

[R49] awk 带条件
来源：http://baike.fanxiaobao.xyz/Article/details/giddynwgj.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.fanxiaobao.xyz/Article/details/gidbxyrtf.sHtML

[R50] awk 求和
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggnwqzoyd.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gmpkikohn.sHtML

[R51] 排序去重取前几
来源：http://3g.fanxiaobao.xyz/Article/details/gmebxslzr.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.fanxiaobao.xyz/Article/details/gxmhbtyvc.sHtML

[R52] 统计行数
来源：http://3g.fanxiaobao.xyz/Article/details/gmnthpgqf.sHtML

wc -l a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkwtydbmg.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.fanxiaobao.xyz/Article/details/gmenxcsjm.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.fanxiaobao.xyz/Article/details/gnlmakfkw.sHtML

[R54] 比较两个文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfusuofgh.sHtML

diff a.txt b.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gjuetgyoy.sHtML

[R55] 压缩与解压
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdevmzses.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.fanxiaobao.xyz/Article/details/glmdzxwio.sHtML

[R56] 远程拷贝
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvttmnjwf.sHtML

scp file user@host:/path/
来源：http://www.blog.fanxiaobao.xyz/Article/details/gghptssrc.sHtML

[R57] 远程执行命令
来源：http://blog.fanxiaobao.xyz/Article/details/gdrsqrbic.sHtML

ssh user@host 'uptime'
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdtqycgjj.sHtML

[R58] 下载文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gwfkuyaiq.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.fanxiaobao.xyz/Article/details/gjohrvaca.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gewnltzuc.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.fanxiaobao.xyz/Article/details/godcbavxp.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.fanxiaobao.xyz/Article/details/gzldmsqir.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.fanxiaobao.xyz/Article/details/gbyxauhch.sHtML

[R61] 磁盘占用
来源：http://www.share.fanxiaobao.xyz/Article/details/gcvyrowkf.sHtML

df -h;  du -sh *
来源：http://mobile.fanxiaobao.xyz/Article/details/glmhtatbk.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzxvquxem.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.fanxiaobao.xyz/Article/details/gmzmpgjbz.sHtML

[R63] 内存与进程
来源：http://baike.fanxiaobao.xyz/Article/details/grrkiegcn.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.fanxiaobao.xyz/Article/details/ggbokvjir.sHtML

[R64] 结束进程
来源：http://read.share.fanxiaobao.xyz/Article/details/gbjwujjdy.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.fanxiaobao.xyz/Article/details/gnyjcgnxb.sHtML

[R65] 查看端口占用
来源：http://wap.fanxiaobao.xyz/Article/details/gehtjnlxj.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.fanxiaobao.xyz/Article/details/gvsnboavg.sHtML

[R66] 定时任务
来源：http://blog.fanxiaobao.xyz/Article/details/gkiskuuzb.sHtML

crontab -e;  crontab -l
来源：http://3g.fanxiaobao.xyz/Article/details/gnqpavnhk.sHtML

[R67] 生成随机十六进制串
来源：http://baike.fanxiaobao.xyz/Article/details/gcrfzttgd.sHtML

openssl rand -hex 16
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goqtrbahd.sHtML

[R68] 计算文件校验值
来源：http://wap.fanxiaobao.xyz/Article/details/ghvkonugy.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/giankqvsw.sHtML

[R69] 生成随机密码
来源：http://baike.fanxiaobao.xyz/Article/details/gbrquftpm.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gookgqyjp.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfenmtopm.sHtML

date +%s;  date -d @1700000000
来源：http://blog.fanxiaobao.xyz/Article/details/gtrnnxemw.sHtML

[R71] 日期格式化
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggbctktvw.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gufzrjusw.sHtML

[R72] 等待端口就绪
来源：http://blog.fanxiaobao.xyz/Article/details/gmzjqawjr.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.fanxiaobao.xyz/Article/details/gypzjkvdp.sHtML

[R73] 分割大日志
来源：http://www.blog.fanxiaobao.xyz/Article/details/goybqxajp.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glpedvfvy.sHtML

[R74] 批量重命名
来源：http://baike.fanxiaobao.xyz/Article/details/gzgkoikey.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gywshirpc.sHtML

[R75] 导出环境变量
来源：http://baike.fanxiaobao.xyz/Article/details/gpbreikvb.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.fanxiaobao.xyz/Article/details/gzrxiktzq.sHtML

[R76] 使用临时文件
来源：http://wap.fanxiaobao.xyz/Article/details/gbfxowmtf.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.fanxiaobao.xyz/Article/details/gdadhhyyr.sHtML

[R77] 读取用户输入
来源：http://blog.fanxiaobao.xyz/Article/details/gmlhrhyky.sHtML

read -rp "请输入: " ans
来源：http://m.share.fanxiaobao.xyz/Article/details/guirtocur.sHtML

[R78] 交互式菜单
来源：http://wap.fanxiaobao.xyz/Article/details/gpaiutovz.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gavlmzukd.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfwnksfja.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gtqrrgasy.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.fanxiaobao.xyz/Article/details/gvkhafilz.sHtML

time ./run.sh
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggwjfmxsa.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gennsrygu.sHtML

S. C / C++ 专题
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxwyhvgzf.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gumfebxvb.sHtML

[S01] C：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxotjbies.sHtML

#include <stdio.h>
来源：http://blog.fanxiaobao.xyz/Article/details/ggacvutwj.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gyjgjftjl.sHtML

[S02] C：变量与格式化输出
来源：http://3g.fanxiaobao.xyz/Article/details/gbprpbxzr.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.fanxiaobao.xyz/Article/details/gfxokaycb.sHtML

[S03] C：读入整数
来源：http://baike.fanxiaobao.xyz/Article/details/gseypldon.sHtML

int x; scanf("%d", &x);
来源：http://wap.fanxiaobao.xyz/Article/details/gqsupgrar.sHtML

[S04] C：字符串复制
来源：http://www.share.fanxiaobao.xyz/Article/details/gxebitkad.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.fanxiaobao.xyz/Article/details/gnfzrncmn.sHtML

[S05] C：字符串长度
来源：http://blog.fanxiaobao.xyz/Article/details/goqbdxmus.sHtML

strlen(s)
来源：http://wap.fanxiaobao.xyz/Article/details/gekqxubba.sHtML

[S06] C：字符串比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfirxnvad.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpdzqfrre.sHtML

[S07] C：数组遍历求和
来源：http://www.share.fanxiaobao.xyz/Article/details/gdroihlgk.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.fanxiaobao.xyz/Article/details/grsbkuokt.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.fanxiaobao.xyz/Article/details/gfrgdoklg.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gacrxilwp.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.fanxiaobao.xyz/Article/details/gmxcakvih.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqhmqowni.sHtML

[S10] C：指针与解引用
来源：http://baike.fanxiaobao.xyz/Article/details/gkaccdwgg.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.fanxiaobao.xyz/Article/details/gtxsmulcp.sHtML

[S11] C：逐行读文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gruzvrxtb.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.fanxiaobao.xyz/Article/details/gbyshtbko.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.fanxiaobao.xyz/Article/details/grenjznsu.sHtML

fclose(f);
来源：http://m.share.fanxiaobao.xyz/Article/details/ggzcoxhjk.sHtML

[S12] C：写文件
来源：http://blog.fanxiaobao.xyz/Article/details/gtfogkyib.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.fanxiaobao.xyz/Article/details/gntpunhgw.sHtML

[S13] C：宏定义
来源：http://3g.fanxiaobao.xyz/Article/details/gyvoopols.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.fanxiaobao.xyz/Article/details/gzxnuklee.sHtML

[S14] C：枚举
来源：http://3g.fanxiaobao.xyz/Article/details/ggppiezjt.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.fanxiaobao.xyz/Article/details/grxlzckge.sHtML

[S15] C：类型转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwrqlezvu.sHtML

(double) a / b
来源：http://baike.fanxiaobao.xyz/Article/details/gcarvltub.sHtML

[S16] C：位操作置位
来源：http://m.share.fanxiaobao.xyz/Article/details/glnbisoda.sHtML

x |= (1 << 3);
来源：http://wap.fanxiaobao.xyz/Article/details/gsyidzmum.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnurwsccs.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.fanxiaobao.xyz/Article/details/geenkpumw.sHtML

[S18] C：命令行参数
来源：http://baike.fanxiaobao.xyz/Article/details/glrtchesv.sHtML

int main(int argc, char **argv)
来源：http://baike.fanxiaobao.xyz/Article/details/gtnsbmmpc.sHtML

[S19] C：快速排序
来源：http://m.share.fanxiaobao.xyz/Article/details/gsfoyymfy.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.fanxiaobao.xyz/Article/details/guckdzczg.sHtML

[S20] C：二分查找
来源：http://mobile.fanxiaobao.xyz/Article/details/gskqgnwxg.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.fanxiaobao.xyz/Article/details/gbcoakixk.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glsepdobs.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.fanxiaobao.xyz/Article/details/gzurzaapc.sHtML

[S22] C：字符串转数字
来源：http://m.share.fanxiaobao.xyz/Article/details/gatjueuuy.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.fanxiaobao.xyz/Article/details/glswboppm.sHtML

[S23] C：随机数
来源：http://mobile.fanxiaobao.xyz/Article/details/gdbegdyxc.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsafslxoh.sHtML

[S24] C：获取本地时间
来源：http://baike.fanxiaobao.xyz/Article/details/gzusapwpp.sHtML


<!-- 参考信息 -->