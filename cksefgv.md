代发 wailian999

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.share.fanxiaobao.xyz/Article/details/gwxpaczjo.sHtML

[Q60] 取上一行 / 下一行
来源：http://baike.fanxiaobao.xyz/Article/details/grzkboadc.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wap.fanxiaobao.xyz/Article/details/gckdhkxkv.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://read.share.fanxiaobao.xyz/Article/details/gqgrpocai.sHtML

[Q61] 移动平均
来源：http://m.share.fanxiaobao.xyz/Article/details/gwkdmloev.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gahbcwgbo.sHtML

[Q62] 分组占比
来源：http://3g.fanxiaobao.xyz/Article/details/grcpjctnl.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.fanxiaobao.xyz/Article/details/gespjezcn.sHtML

[Q63] 开启事务
来源：http://read.share.fanxiaobao.xyz/Article/details/gvsknkdcc.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.share.fanxiaobao.xyz/Article/details/gvmbipgpg.sHtML

[Q64] 提交事务
来源：http://baike.fanxiaobao.xyz/Article/details/gfrtgytsj.sHtML

COMMIT;
来源：http://read.share.fanxiaobao.xyz/Article/details/gickcjmzk.sHtML

[Q65] 回滚事务
来源：http://mobile.fanxiaobao.xyz/Article/details/gekiyffmv.sHtML

ROLLBACK;
来源：http://www.share.fanxiaobao.xyz/Article/details/gbkzjedlm.sHtML

[Q66] 行锁查询
来源：http://m.share.fanxiaobao.xyz/Article/details/gcnqcmfcv.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpppckzgr.sHtML

[Q67] 设置隔离级别
来源：http://3g.fanxiaobao.xyz/Article/details/geydnxunq.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmpakghan.sHtML

[Q68] 保存点
来源：http://www.blog.fanxiaobao.xyz/Article/details/glrydoovd.sHtML

SAVEPOINT sp1;
来源：http://wap.fanxiaobao.xyz/Article/details/gluoqwyea.sHtML

ROLLBACK TO sp1;
来源：http://baike.fanxiaobao.xyz/Article/details/gafmfomvy.sHtML

[Q69] 查看执行计划
来源：http://3g.fanxiaobao.xyz/Article/details/gziyeamtv.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://baike.fanxiaobao.xyz/Article/details/ggsdbclsy.sHtML

[Q70] 更新统计信息
来源：http://3g.fanxiaobao.xyz/Article/details/gdhekuzjv.sHtML

ANALYZE TABLE users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gafwhjlzg.sHtML

[Q71] 查看建表语句
来源：http://read.share.fanxiaobao.xyz/Article/details/gowisqbrz.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.blog.fanxiaobao.xyz/Article/details/grtglctoq.sHtML

[Q72] 查看索引
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjxxgsfjx.sHtML

SHOW INDEX FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggnunxhmf.sHtML

[Q73] 查看表状态
来源：http://www.share.fanxiaobao.xyz/Article/details/gwcffggpg.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://baike.fanxiaobao.xyz/Article/details/gaeidpfwz.sHtML

[Q74] 强制使用索引
来源：http://read.share.fanxiaobao.xyz/Article/details/gyssdbaaz.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://blog.fanxiaobao.xyz/Article/details/gpgrmryis.sHtML

[Q75] 日期格式化
来源：http://read.share.fanxiaobao.xyz/Article/details/glaoxcbkq.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mobile.fanxiaobao.xyz/Article/details/gmphmehoc.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.fanxiaobao.xyz/Article/details/gcdzxmhia.sHtML

[Q76] 按天统计
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gshpuvvpr.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://blog.fanxiaobao.xyz/Article/details/ghnmrqcqo.sHtML

[Q77] 时间加减
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtejnxral.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://m.share.fanxiaobao.xyz/Article/details/gzixtmvkc.sHtML

[Q78] 当前时间
来源：http://blog.fanxiaobao.xyz/Article/details/gibfcswfo.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.blog.fanxiaobao.xyz/Article/details/gztlesrex.sHtML

[Q79] 字符串拼接
来源：http://www.share.fanxiaobao.xyz/Article/details/ggcsezswe.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.fanxiaobao.xyz/Article/details/gckpbkfsl.sHtML

[Q80] 字符串截取
来源：http://read.share.fanxiaobao.xyz/Article/details/gyaixjwlw.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfvdedceb.sHtML

[Q81] 字符串替换
来源：http://mobile.fanxiaobao.xyz/Article/details/guvkosppj.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gctfaafes.sHtML

[Q82] 字符长度与字节长度
来源：http://m.share.fanxiaobao.xyz/Article/details/gyldfepzl.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gvcqiuxmr.sHtML

[Q83] 大小写转换
来源：http://www.share.fanxiaobao.xyz/Article/details/gbkiadljq.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gggpaycps.sHtML

[Q84] 去除首尾空格
来源：http://blog.fanxiaobao.xyz/Article/details/gwlxgfwph.sHtML

SELECT TRIM(name) FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gcksooaot.sHtML

[Q85] 数值取整
来源：http://www.share.fanxiaobao.xyz/Article/details/gxnrjgavg.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wap.fanxiaobao.xyz/Article/details/gophyacns.sHtML

[Q86] 读取 JSON 字段
来源：http://www.share.fanxiaobao.xyz/Article/details/grkwfytkk.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.fanxiaobao.xyz/Article/details/gydtsynwa.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.fanxiaobao.xyz/Article/details/gavbpdbsv.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.fanxiaobao.xyz/Article/details/gidsbztvu.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.fanxiaobao.xyz/Article/details/gxrcakjsu.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.fanxiaobao.xyz/Article/details/gdsdxvnwc.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gdwkhhzdy.sHtML

[Q89] 判断表是否存在
来源：http://baike.fanxiaobao.xyz/Article/details/gadpqknoc.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzmanngrn.sHtML

[Q90] 生成序号列
来源：http://mobile.fanxiaobao.xyz/Article/details/gvjrfdlhm.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.fanxiaobao.xyz/Article/details/gjqhxbils.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gdlgfsujf.sHtML

R. Bash 专题
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmttqhxfr.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/glczlvaqy.sHtML

[R01] shebang 与严格模式
来源：http://mobile.fanxiaobao.xyz/Article/details/geelmwyqo.sHtML

#!/usr/bin/env bash
来源：http://blog.fanxiaobao.xyz/Article/details/gkdoxnmcu.sHtML

set -euo pipefail
来源：http://www.share.fanxiaobao.xyz/Article/details/gchhewnzd.sHtML

[R02] 变量赋值与使用
来源：http://www.share.fanxiaobao.xyz/Article/details/gwdvgihvm.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.fanxiaobao.xyz/Article/details/glfthiuep.sHtML

[R03] 只读变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gyrgpsmih.sHtML

readonly PI=3.14
来源：http://wap.fanxiaobao.xyz/Article/details/ghglaqwzd.sHtML

[R04] 位置参数
来源：http://read.share.fanxiaobao.xyz/Article/details/gdzoibshf.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.fanxiaobao.xyz/Article/details/gcyrqwbig.sHtML

[R05] 参数默认值
来源：http://3g.fanxiaobao.xyz/Article/details/gmipsztev.sHtML

name="${1:-default}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gypuprryn.sHtML

[R06] 判断命令是否存在
来源：http://m.share.fanxiaobao.xyz/Article/details/gowihfvtl.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.fanxiaobao.xyz/Article/details/gjwuyaolo.sHtML

[R07] if 判断文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gfbqfrdme.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.fanxiaobao.xyz/Article/details/gnxkrbzoa.sHtML

[R08] 数值比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghpbnoaor.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://wap.fanxiaobao.xyz/Article/details/gmtrdihau.sHtML

[R09] 字符串比较
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkgaraawt.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.fanxiaobao.xyz/Article/details/gscucpvys.sHtML

[R10] 正则匹配
来源：http://m.share.fanxiaobao.xyz/Article/details/gtswwsfyo.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcznlvbgw.sHtML

[R11] case 多分支
来源：http://www.share.fanxiaobao.xyz/Article/details/gsjqkswbn.sHtML

case "$1" in
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzifkybdc.sHtML

start) echo "启动" ;;
来源：http://mobile.fanxiaobao.xyz/Article/details/gnpuysjqf.sHtML

stop)  echo "停止" ;;
来源：http://read.share.fanxiaobao.xyz/Article/details/gjynkjpah.sHtML

*)     echo "未知命令" ;;
来源：http://baike.fanxiaobao.xyz/Article/details/grkqalumq.sHtML

esac
来源：http://www.blog.fanxiaobao.xyz/Article/details/gytggkvgv.sHtML

[R12] for 遍历文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gvibvupop.sHtML

for f in *.txt; do echo "$f"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gdldxrkuw.sHtML

[R13] for 计数循环
来源：http://www.blog.fanxiaobao.xyz/Article/details/grcgvhqze.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.fanxiaobao.xyz/Article/details/gvehfoxak.sHtML

[R14] C 风格 for
来源：http://read.share.fanxiaobao.xyz/Article/details/gtnwrrezn.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/ghmahfrkh.sHtML

[R15] while 逐行读文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gkslbtpqg.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gotqilgyi.sHtML

[R16] until 等待条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gptgkqodd.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gooaufjsl.sHtML

[R17] 数组定义与取值
来源：http://baike.fanxiaobao.xyz/Article/details/gguwvcejx.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.fanxiaobao.xyz/Article/details/glyvsdtsu.sHtML

[R18] 遍历数组
来源：http://mobile.fanxiaobao.xyz/Article/details/grklnmhla.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.fanxiaobao.xyz/Article/details/grdaadfgs.sHtML

[R19] 数组长度
来源：http://mobile.fanxiaobao.xyz/Article/details/gxdgizocd.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glesfjnft.sHtML

[R20] 关联数组（字典）
来源：http://m.share.fanxiaobao.xyz/Article/details/gmouwhawg.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.fanxiaobao.xyz/Article/details/guorgjvdv.sHtML

[R21] 字符串长度
来源：http://baike.fanxiaobao.xyz/Article/details/gddjcmbyc.sHtML

echo "${#s}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxilahzcm.sHtML

[R22] 截取子串
来源：http://mobile.fanxiaobao.xyz/Article/details/giqlfpowl.sHtML

echo "${s:0:5}"
来源：http://blog.fanxiaobao.xyz/Article/details/gllvuragy.sHtML

[R23] 字符串替换
来源：http://baike.fanxiaobao.xyz/Article/details/gcexlfphc.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.fanxiaobao.xyz/Article/details/ghcgaqtgr.sHtML

[R24] 大小写转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxwllhnxs.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gctpdfaho.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.fanxiaobao.xyz/Article/details/gihlddngi.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.fanxiaobao.xyz/Article/details/grmfviokk.sHtML

[R26] 命令替换
来源：http://blog.fanxiaobao.xyz/Article/details/goecgpors.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.fanxiaobao.xyz/Article/details/ggwurzqfv.sHtML

[R27] 算术展开
来源：http://www.share.fanxiaobao.xyz/Article/details/gkrunwvrk.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.fanxiaobao.xyz/Article/details/gjiodzecu.sHtML

[R28] 浮点运算
来源：http://read.share.fanxiaobao.xyz/Article/details/gxtmrlafa.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.fanxiaobao.xyz/Article/details/gbxqotark.sHtML

[R29] 定义函数
来源：http://baike.fanxiaobao.xyz/Article/details/gveozdxoy.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.fanxiaobao.xyz/Article/details/gqshhiecz.sHtML

[R30] 函数返回状态码
来源：http://www.share.fanxiaobao.xyz/Article/details/gyrhxjfvz.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.fanxiaobao.xyz/Article/details/grdxdpxsg.sHtML

[R31] 局部变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gyhlwqyan.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gzcfhgakv.sHtML

[R32] 参数个数校验
来源：http://read.share.fanxiaobao.xyz/Article/details/giglozlam.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.fanxiaobao.xyz/Article/details/gaecjoiqw.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.fanxiaobao.xyz/Article/details/gtdeclxkz.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.fanxiaobao.xyz/Article/details/gzomsfprq.sHtML

[R34] 退出时清理
来源：http://baike.fanxiaobao.xyz/Article/details/grvhfehzr.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fanxiaobao.xyz/Article/details/gomsftwzy.sHtML

[R35] 后台执行并等待
来源：http://baike.fanxiaobao.xyz/Article/details/ghuiidigf.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gexqrbgyh.sHtML

[R36] 并发执行多个任务
来源：http://baike.fanxiaobao.xyz/Article/details/gbxhsayag.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpdmhtfsu.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gylhurhal.sHtML

files=$(ls -1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gczfavovl.sHtML

[R38] 管道串联
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gstqvaqrv.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.fanxiaobao.xyz/Article/details/gbanexytb.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.fanxiaobao.xyz/Article/details/gymrydnvs.sHtML

cmd > out.log 2>&1
来源：http://blog.fanxiaobao.xyz/Article/details/ghmohfvov.sHtML

[R40] 追加写日志
来源：http://mobile.fanxiaobao.xyz/Article/details/ghwzjdjxu.sHtML

echo "log" >> out.log
来源：http://blog.fanxiaobao.xyz/Article/details/gcgdmrzlw.sHtML

[R41] 丢弃输出
来源：http://3g.fanxiaobao.xyz/Article/details/gunxgnhxj.sHtML

cmd >/dev/null 2>&1
来源：http://baike.fanxiaobao.xyz/Article/details/gwaxexnte.sHtML

[R42] 输入重定向
来源：http://read.share.fanxiaobao.xyz/Article/details/gzmeanmwh.sHtML

wc -l < a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gtinhotcf.sHtML

[R43] 按名字查找文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gocsoiupx.sHtML

find . -name "*.log" -type f
来源：http://www.share.fanxiaobao.xyz/Article/details/goavfwnbw.sHtML

[R44] 按修改时间查找
来源：http://baike.fanxiaobao.xyz/Article/details/gnalzuozs.sHtML

find . -mtime -7 -type f
来源：http://read.share.fanxiaobao.xyz/Article/details/gwazbvnbl.sHtML

[R45] 批量删除
来源：http://3g.fanxiaobao.xyz/Article/details/gmzztkdcm.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.fanxiaobao.xyz/Article/details/gnensvlkb.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gslqpmcaf.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.fanxiaobao.xyz/Article/details/gubkvghmb.sHtML

[R47] sed 单行替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtaskpxqo.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gnnqwment.sHtML

[R48] awk 取指定列
来源：http://m.share.fanxiaobao.xyz/Article/details/gqkaboovh.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gytkfeqmv.sHtML

[R49] awk 带条件
来源：http://m.share.fanxiaobao.xyz/Article/details/ghvgmpwfn.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.fanxiaobao.xyz/Article/details/gjocsoplg.sHtML

[R50] awk 求和
来源：http://blog.fanxiaobao.xyz/Article/details/gvezeuhiy.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/ggepuhyvr.sHtML

[R51] 排序去重取前几
来源：http://baike.fanxiaobao.xyz/Article/details/gweikwzpy.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.fanxiaobao.xyz/Article/details/gbzveetlw.sHtML

[R52] 统计行数
来源：http://wap.fanxiaobao.xyz/Article/details/guzyzlims.sHtML

wc -l a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gldbndzte.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.fanxiaobao.xyz/Article/details/gxastqpje.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.fanxiaobao.xyz/Article/details/gjisueiyy.sHtML

[R54] 比较两个文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gocxoakvi.sHtML

diff a.txt b.txt
来源：http://wap.fanxiaobao.xyz/Article/details/glmloyfot.sHtML

[R55] 压缩与解压
来源：http://3g.fanxiaobao.xyz/Article/details/geepzfmic.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.fanxiaobao.xyz/Article/details/gulgmybjq.sHtML

[R56] 远程拷贝
来源：http://read.share.fanxiaobao.xyz/Article/details/gljoedzwo.sHtML

scp file user@host:/path/
来源：http://mobile.fanxiaobao.xyz/Article/details/gjsgxwahv.sHtML

[R57] 远程执行命令
来源：http://baike.fanxiaobao.xyz/Article/details/gxtrrocnz.sHtML

ssh user@host 'uptime'
来源：http://www.blog.fanxiaobao.xyz/Article/details/grfvndybk.sHtML

[R58] 下载文件
来源：http://wap.fanxiaobao.xyz/Article/details/gnwldysav.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.fanxiaobao.xyz/Article/details/gjqvgfmzn.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gycgjbvse.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.fanxiaobao.xyz/Article/details/gatljwttd.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.fanxiaobao.xyz/Article/details/gbchiwmby.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.fanxiaobao.xyz/Article/details/gaopuockf.sHtML

[R61] 磁盘占用
来源：http://blog.fanxiaobao.xyz/Article/details/gumjejldv.sHtML

df -h;  du -sh *
来源：http://3g.fanxiaobao.xyz/Article/details/gvwefiexa.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaaiwefyk.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.fanxiaobao.xyz/Article/details/gvkocyuwr.sHtML

[R63] 内存与进程
来源：http://3g.fanxiaobao.xyz/Article/details/gkcqvkfle.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.fanxiaobao.xyz/Article/details/gvdgusrub.sHtML

[R64] 结束进程
来源：http://baike.fanxiaobao.xyz/Article/details/gwnoegyou.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.fanxiaobao.xyz/Article/details/gwkxwulvx.sHtML

[R65] 查看端口占用
来源：http://wap.fanxiaobao.xyz/Article/details/gtezsclyq.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.fanxiaobao.xyz/Article/details/gmblticzv.sHtML

[R66] 定时任务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtcgrkjfi.sHtML

crontab -e;  crontab -l
来源：http://www.blog.fanxiaobao.xyz/Article/details/grzknaibw.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnwjnylap.sHtML

openssl rand -hex 16
来源：http://wap.fanxiaobao.xyz/Article/details/gfozlfixo.sHtML

[R68] 计算文件校验值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbxsxsqxk.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gbrcbgvpm.sHtML

[R69] 生成随机密码
来源：http://www.blog.fanxiaobao.xyz/Article/details/ganhxyjof.sHtML

head -c 16 /dev/urandom | base64
来源：http://read.share.fanxiaobao.xyz/Article/details/gurazqhce.sHtML

[R70] 时间戳与互转
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsdbyseac.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.fanxiaobao.xyz/Article/details/glamvlxaa.sHtML

[R71] 日期格式化
来源：http://www.share.fanxiaobao.xyz/Article/details/gejpzgrjr.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.fanxiaobao.xyz/Article/details/gheyekgfy.sHtML

[R72] 等待端口就绪
来源：http://blog.fanxiaobao.xyz/Article/details/ggyhhqvin.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.fanxiaobao.xyz/Article/details/gofxhfmsy.sHtML

[R73] 分割大日志
来源：http://read.share.fanxiaobao.xyz/Article/details/gyhhdgqzo.sHtML

split -l 1000 big.log part_
来源：http://3g.fanxiaobao.xyz/Article/details/gyyxaytmc.sHtML

[R74] 批量重命名
来源：http://read.share.fanxiaobao.xyz/Article/details/gdrspazvf.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmncibfix.sHtML

[R75] 导出环境变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gxqjpvqxa.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.fanxiaobao.xyz/Article/details/gdzfmsqxc.sHtML

[R76] 使用临时文件
来源：http://3g.fanxiaobao.xyz/Article/details/gqukceryd.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.fanxiaobao.xyz/Article/details/gtgrhfyrc.sHtML

[R77] 读取用户输入
来源：http://mobile.fanxiaobao.xyz/Article/details/gzmjijddm.sHtML

read -rp "请输入: " ans
来源：http://blog.fanxiaobao.xyz/Article/details/gfvjwvvth.sHtML

[R78] 交互式菜单
来源：http://m.share.fanxiaobao.xyz/Article/details/gletaleok.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gwdnrizce.sHtML

[R79] 解析命令行选项
来源：http://www.blog.fanxiaobao.xyz/Article/details/giasnhimm.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.fanxiaobao.xyz/Article/details/grnkhafhh.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.fanxiaobao.xyz/Article/details/gwqjwizyb.sHtML

time ./run.sh
来源：http://www.share.fanxiaobao.xyz/Article/details/gbdtbpgmx.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gurfdwmia.sHtML

S. C / C++ 专题
来源：http://blog.fanxiaobao.xyz/Article/details/ggkaoeqos.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/ghszzznls.sHtML

[S01] C：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyqcfgmrg.sHtML

#include <stdio.h>
来源：http://wap.fanxiaobao.xyz/Article/details/gwenhjgin.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gqyyrxiys.sHtML

[S02] C：变量与格式化输出
来源：http://blog.fanxiaobao.xyz/Article/details/gighwftfh.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.fanxiaobao.xyz/Article/details/ggqphglic.sHtML

[S03] C：读入整数
来源：http://mobile.fanxiaobao.xyz/Article/details/goyxsguxd.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjtddnpkr.sHtML

[S04] C：字符串复制
来源：http://www.share.fanxiaobao.xyz/Article/details/gheicsdhk.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.fanxiaobao.xyz/Article/details/gpvflrytd.sHtML

[S05] C：字符串长度
来源：http://m.share.fanxiaobao.xyz/Article/details/gjulcowjm.sHtML

strlen(s)
来源：http://blog.fanxiaobao.xyz/Article/details/ghyyplxep.sHtML

[S06] C：字符串比较
来源：http://www.share.fanxiaobao.xyz/Article/details/gmsccxsif.sHtML

strcmp(a, b) == 0
来源：http://wap.fanxiaobao.xyz/Article/details/gqukvstgu.sHtML

[S07] C：数组遍历求和
来源：http://baike.fanxiaobao.xyz/Article/details/ggzweryqi.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.fanxiaobao.xyz/Article/details/gwhvnpfzw.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjupjpmpe.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.fanxiaobao.xyz/Article/details/gaoxwsbtd.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.fanxiaobao.xyz/Article/details/gtjgjixth.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.fanxiaobao.xyz/Article/details/ggacrrnfk.sHtML

[S10] C：指针与解引用
来源：http://www.blog.fanxiaobao.xyz/Article/details/gboesydkx.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.fanxiaobao.xyz/Article/details/gbbxnlwac.sHtML

[S11] C：逐行读文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggtymxgav.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gostcalns.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.fanxiaobao.xyz/Article/details/ghbosqhtj.sHtML

fclose(f);
来源：http://m.share.fanxiaobao.xyz/Article/details/gklqzmebc.sHtML

[S12] C：写文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gvcvsarsn.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.fanxiaobao.xyz/Article/details/ghlfwzgcy.sHtML

[S13] C：宏定义
来源：http://m.share.fanxiaobao.xyz/Article/details/gtbtgzdsn.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.fanxiaobao.xyz/Article/details/gbfagasqi.sHtML

[S14] C：枚举
来源：http://blog.fanxiaobao.xyz/Article/details/gygrczczn.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.fanxiaobao.xyz/Article/details/gjcroijzd.sHtML

[S15] C：类型转换
来源：http://3g.fanxiaobao.xyz/Article/details/gbizvjazc.sHtML

(double) a / b
来源：http://m.share.fanxiaobao.xyz/Article/details/gqhtmfoiz.sHtML

[S16] C：位操作置位
来源：http://blog.fanxiaobao.xyz/Article/details/gkedccnwl.sHtML

x |= (1 << 3);
来源：http://www.share.fanxiaobao.xyz/Article/details/ggztdixlp.sHtML

[S17] C：安全拼接字符串
来源：http://baike.fanxiaobao.xyz/Article/details/guhgqdubb.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.fanxiaobao.xyz/Article/details/gdxkvnzup.sHtML

[S18] C：命令行参数
来源：http://read.share.fanxiaobao.xyz/Article/details/ggqnekhxb.sHtML

int main(int argc, char **argv)
来源：http://www.blog.fanxiaobao.xyz/Article/details/grgsqvpzd.sHtML

[S19] C：快速排序
来源：http://www.share.fanxiaobao.xyz/Article/details/gfdrflshy.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.fanxiaobao.xyz/Article/details/gidguunva.sHtML

[S20] C：二分查找
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfgjtmtrd.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.fanxiaobao.xyz/Article/details/gzzwrvfft.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gajlekhdu.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.fanxiaobao.xyz/Article/details/gbqoodiii.sHtML

[S22] C：字符串转数字
来源：http://wap.fanxiaobao.xyz/Article/details/gasmbwtpc.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.fanxiaobao.xyz/Article/details/gtttlwlpv.sHtML

[S23] C：随机数
来源：http://3g.fanxiaobao.xyz/Article/details/guwlpjsup.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.fanxiaobao.xyz/Article/details/gafngrgku.sHtML

[S24] C：获取本地时间
来源：http://m.share.fanxiaobao.xyz/Article/details/gitrkuffh.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.fanxiaobao.xyz/Article/details/gshrkpioa.sHtML

[S25] C：内存拷贝
来源：http://m.share.fanxiaobao.xyz/Article/details/grbjdikdv.sHtML

memcpy(dst, src, n);
来源：http://mobile.fanxiaobao.xyz/Article/details/gxjowojvs.sHtML

[S26] C：内存清零
来源：http://3g.fanxiaobao.xyz/Article/details/gbklpymsv.sHtML

memset(a, 0, sizeof a);
来源：http://wap.fanxiaobao.xyz/Article/details/gwmzmusqz.sHtML

[S27] C：定义常量
来源：http://wap.fanxiaobao.xyz/Article/details/giulfdjek.sHtML

const double PI = 3.14159;
来源：http://read.share.fanxiaobao.xyz/Article/details/ghthvfirq.sHtML

[S28] C：静态变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfzvexrnk.sHtML

static int counter = 0;
来源：http://m.share.fanxiaobao.xyz/Article/details/glksdxngi.sHtML

[S29] C：变参函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gapnpmrga.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnlrigrpg.sHtML

[S30] C：头文件保护
来源：http://www.blog.fanxiaobao.xyz/Article/details/goaqpifvd.sHtML


<!-- 参考信息 -->