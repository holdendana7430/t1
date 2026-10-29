代发 wailian999

[Q67] 设置隔离级别
来源：http://blog.hesvh.cn/Article/details/gmhfagrjh.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://baike.hesvh.cn/Article/details/gakuunwvu.sHtML

[Q68] 保存点
来源：http://baike.fehbvm.com/Article/details/gkzkjfooz.sHtML

SAVEPOINT sp1;
来源：http://m.share.hesvh.cn/Article/details/gwrfgmrik.sHtML

ROLLBACK TO sp1;
来源：http://3g.fehbvm.com/Article/details/gqmcbdewt.sHtML

[Q69] 查看执行计划
来源：http://wap.fehbvm.com/Article/details/gsiymekai.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.m.share.zdbjq.cn/Article/details/gnkmdetjr.sHtML

[Q70] 更新统计信息
来源：http://3g.hesvh.cn/Article/details/gkarmmhvq.sHtML

ANALYZE TABLE users;
来源：http://mobile.zdbjq.cn/Article/details/gpmjstdfy.sHtML

[Q71] 查看建表语句
来源：http://baike.zdbjq.cn/Article/details/gxpizvoza.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.fehbvm.com/Article/details/gdyspvnwa.sHtML

[Q72] 查看索引
来源：http://read.share.fehbvm.com/Article/details/gkpdaufaf.sHtML

SHOW INDEX FROM users;
来源：http://3g.hesvh.cn/Article/details/grnhwjfts.sHtML

[Q73] 查看表状态
来源：http://baike.zdbjq.cn/Article/details/gjdtwogwa.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://read.share.zdbjq.cn/Article/details/gocyjkbkw.sHtML

[Q74] 强制使用索引
来源：http://3g.hesvh.cn/Article/details/gzxjodwbg.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://read.share.fehbvm.com/Article/details/gzhhusuzg.sHtML

[Q75] 日期格式化
来源：http://m.share.fehbvm.com/Article/details/ggdptwnxi.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://read.share.zdbjq.cn/Article/details/gkmrqacwk.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.hesvh.cn/Article/details/gtvqkffod.sHtML

[Q76] 按天统计
来源：http://mobile.hesvh.cn/Article/details/gtghmedpq.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://3g.hesvh.cn/Article/details/gpubzktxf.sHtML

[Q77] 时间加减
来源：http://www.blog.fehbvm.com/Article/details/ggblsazbl.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.hesvh.cn/Article/details/gsyximmrd.sHtML

[Q78] 当前时间
来源：http://www.m.share.fehbvm.com/Article/details/gcfvsmddi.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.m.share.hesvh.cn/Article/details/gxfuorxfx.sHtML

[Q79] 字符串拼接
来源：http://www.share.fehbvm.com/Article/details/gockmrrnc.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.hesvh.cn/Article/details/greikbtmp.sHtML

[Q80] 字符串截取
来源：http://blog.fehbvm.com/Article/details/gftqwmrck.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gadxkbeqt.sHtML

[Q81] 字符串替换
来源：http://www.m.share.zdbjq.cn/Article/details/gtgvmnydx.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.fehbvm.com/Article/details/gbiedugzr.sHtML

[Q82] 字符长度与字节长度
来源：http://3g.zdbjq.cn/Article/details/ghzxdkpcr.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gsphqknex.sHtML

[Q83] 大小写转换
来源：http://wap.zdbjq.cn/Article/details/gnuguqdjf.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wap.fehbvm.com/Article/details/gpszonhjb.sHtML

[Q84] 去除首尾空格
来源：http://blog.zdbjq.cn/Article/details/gdnhlhlyd.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.hesvh.cn/Article/details/galjilbns.sHtML

[Q85] 数值取整
来源：http://read.share.fehbvm.com/Article/details/gbagwhkwj.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.hesvh.cn/Article/details/gnoxwcxku.sHtML

[Q86] 读取 JSON 字段
来源：http://www.share.fehbvm.com/Article/details/gwiytackr.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://blog.fehbvm.com/Article/details/goanoikwu.sHtML

[Q87] JSON 字段做条件
来源：http://3g.zdbjq.cn/Article/details/gwefocuwz.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.blog.hesvh.cn/Article/details/gftmzeioy.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.m.share.fehbvm.com/Article/details/ghzgvppfm.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.hesvh.cn/Article/details/gvqulcent.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gynaldxej.sHtML

[Q89] 判断表是否存在
来源：http://mobile.hesvh.cn/Article/details/gtutpjhna.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.hesvh.cn/Article/details/gsbgnumsa.sHtML

[Q90] 生成序号列
来源：http://3g.hesvh.cn/Article/details/gxfsycmpn.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://3g.zdbjq.cn/Article/details/gkvoqtzbz.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gnlbzoxzp.sHtML

R. Bash 专题
来源：http://blog.hesvh.cn/Article/details/gmoysqstd.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gagfmerki.sHtML

[R01] shebang 与严格模式
来源：http://mobile.hesvh.cn/Article/details/grgperazg.sHtML

#!/usr/bin/env bash
来源：http://www.share.zdbjq.cn/Article/details/gnkkxxfkg.sHtML

set -euo pipefail
来源：http://www.blog.zdbjq.cn/Article/details/guaibumrd.sHtML

[R02] 变量赋值与使用
来源：http://baike.zdbjq.cn/Article/details/gwevwfiwl.sHtML

name="Tom"; echo "$name"
来源：http://wap.hesvh.cn/Article/details/geupulvcq.sHtML

[R03] 只读变量
来源：http://wap.zdbjq.cn/Article/details/gwbxjisag.sHtML

readonly PI=3.14
来源：http://baike.fehbvm.com/Article/details/gpogsiclz.sHtML

[R04] 位置参数
来源：http://blog.fehbvm.com/Article/details/gyjvjluvy.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.hesvh.cn/Article/details/glqxazunk.sHtML

[R05] 参数默认值
来源：http://www.share.zdbjq.cn/Article/details/gjqkeimyi.sHtML

name="${1:-default}"
来源：http://mobile.fehbvm.com/Article/details/gjibemlqn.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.fehbvm.com/Article/details/goetbibaa.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.hesvh.cn/Article/details/gjfbuityw.sHtML

[R07] if 判断文件
来源：http://3g.fehbvm.com/Article/details/gnyezskth.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://baike.fehbvm.com/Article/details/gpslfeppe.sHtML

[R08] 数值比较
来源：http://mobile.zdbjq.cn/Article/details/glotsdilf.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.hesvh.cn/Article/details/gvpqehmwh.sHtML

[R09] 字符串比较
来源：http://www.blog.hesvh.cn/Article/details/gwmhkncrz.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.zdbjq.cn/Article/details/glxgespzd.sHtML

[R10] 正则匹配
来源：http://3g.zdbjq.cn/Article/details/ghjvdbpds.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.hesvh.cn/Article/details/gpnuwqdhn.sHtML

[R11] case 多分支
来源：http://www.blog.fehbvm.com/Article/details/gpidhmbbd.sHtML

case "$1" in
来源：http://baike.fehbvm.com/Article/details/gbfqnwdrh.sHtML

start) echo "启动" ;;
来源：http://read.share.fehbvm.com/Article/details/gytxbjkmp.sHtML

stop)  echo "停止" ;;
来源：http://wap.fehbvm.com/Article/details/ggsrpkpec.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.hesvh.cn/Article/details/gicqhgiwo.sHtML

esac
来源：http://read.share.fehbvm.com/Article/details/ghkpjjjkz.sHtML

[R12] for 遍历文件
来源：http://wap.zdbjq.cn/Article/details/ghqepwawh.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.zdbjq.cn/Article/details/gkhcqcgpz.sHtML

[R13] for 计数循环
来源：http://wap.fehbvm.com/Article/details/gfqpgdqee.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.m.share.hesvh.cn/Article/details/gbxqiqxrp.sHtML

[R14] C 风格 for
来源：http://www.blog.fehbvm.com/Article/details/gfkwwzvhe.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.zdbjq.cn/Article/details/gtbjbmcdr.sHtML

[R15] while 逐行读文件
来源：http://www.share.fehbvm.com/Article/details/gsvtaqouf.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.zdbjq.cn/Article/details/grxpkpidp.sHtML

[R16] until 等待条件
来源：http://wap.hesvh.cn/Article/details/ghhndlkco.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.fehbvm.com/Article/details/gaanjvbqt.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.fehbvm.com/Article/details/gllwwxosr.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.zdbjq.cn/Article/details/glzwhukkw.sHtML

[R18] 遍历数组
来源：http://read.share.zdbjq.cn/Article/details/giftxzbsy.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.hesvh.cn/Article/details/ggfifhevi.sHtML

[R19] 数组长度
来源：http://blog.hesvh.cn/Article/details/gyzqgmcso.sHtML

echo "${#arr[@]}"
来源：http://read.share.zdbjq.cn/Article/details/gunxuouml.sHtML

[R20] 关联数组（字典）
来源：http://m.share.fehbvm.com/Article/details/ggxuyntof.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mobile.fehbvm.com/Article/details/glemfgymr.sHtML

[R21] 字符串长度
来源：http://3g.fehbvm.com/Article/details/gqxgqzyfl.sHtML

echo "${#s}"
来源：http://wap.hesvh.cn/Article/details/gfqlrepnb.sHtML

[R22] 截取子串
来源：http://www.blog.fehbvm.com/Article/details/gvflbktpw.sHtML

echo "${s:0:5}"
来源：http://3g.fehbvm.com/Article/details/gceitevmv.sHtML

[R23] 字符串替换
来源：http://m.share.hesvh.cn/Article/details/gbjnpzyqh.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.fehbvm.com/Article/details/gafboxksg.sHtML

[R24] 大小写转换
来源：http://m.share.hesvh.cn/Article/details/gpjdznmrz.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.hesvh.cn/Article/details/gsddrscvn.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.zdbjq.cn/Article/details/gomvqbsbm.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.zdbjq.cn/Article/details/gbjptdgpw.sHtML

[R26] 命令替换
来源：http://read.share.zdbjq.cn/Article/details/gdjaafviw.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.fehbvm.com/Article/details/gzffoxdon.sHtML

[R27] 算术展开
来源：http://www.m.share.zdbjq.cn/Article/details/gdcwksxnd.sHtML

echo $((1 + 2 * 3))
来源：http://blog.zdbjq.cn/Article/details/guoghawac.sHtML

[R28] 浮点运算
来源：http://read.share.hesvh.cn/Article/details/gyeoozfze.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.fehbvm.com/Article/details/gvhdxrkyk.sHtML

[R29] 定义函数
来源：http://www.blog.zdbjq.cn/Article/details/gcpuralny.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.fehbvm.com/Article/details/givbttdoe.sHtML

[R30] 函数返回状态码
来源：http://www.blog.zdbjq.cn/Article/details/gpmklzhqv.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.fehbvm.com/Article/details/gfszcpzxx.sHtML

[R31] 局部变量
来源：http://wap.zdbjq.cn/Article/details/gucdekvsa.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.hesvh.cn/Article/details/guykjzbgu.sHtML

[R32] 参数个数校验
来源：http://www.share.fehbvm.com/Article/details/gqqmkzdtv.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.hesvh.cn/Article/details/geyjntlff.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.fehbvm.com/Article/details/gxqnzeopu.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.hesvh.cn/Article/details/glwjjdlzc.sHtML

[R34] 退出时清理
来源：http://mobile.zdbjq.cn/Article/details/gnyzcfavn.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.share.fehbvm.com/Article/details/gweozciuz.sHtML

[R35] 后台执行并等待
来源：http://m.share.fehbvm.com/Article/details/ghqycxryk.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.fehbvm.com/Article/details/gptbrhusn.sHtML

[R36] 并发执行多个任务
来源：http://baike.hesvh.cn/Article/details/grlrrndig.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.fehbvm.com/Article/details/gdropuicc.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.fehbvm.com/Article/details/gpqofyixg.sHtML

files=$(ls -1)
来源：http://read.share.zdbjq.cn/Article/details/gchujuumz.sHtML

[R38] 管道串联
来源：http://blog.fehbvm.com/Article/details/grlyfraql.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.zdbjq.cn/Article/details/gutpglczz.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.hesvh.cn/Article/details/giebflysz.sHtML

cmd > out.log 2>&1
来源：http://3g.hesvh.cn/Article/details/gtcqoltmp.sHtML

[R40] 追加写日志
来源：http://3g.fehbvm.com/Article/details/ghkrnargi.sHtML

echo "log" >> out.log
来源：http://mobile.zdbjq.cn/Article/details/gvcvithja.sHtML

[R41] 丢弃输出
来源：http://m.share.fehbvm.com/Article/details/gcqremkty.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.hesvh.cn/Article/details/gxfvcepae.sHtML

[R42] 输入重定向
来源：http://m.share.fehbvm.com/Article/details/ghaupglkt.sHtML

wc -l < a.txt
来源：http://www.share.zdbjq.cn/Article/details/girxyphdy.sHtML

[R43] 按名字查找文件
来源：http://read.share.hesvh.cn/Article/details/gnyqnzyhp.sHtML

find . -name "*.log" -type f
来源：http://mobile.fehbvm.com/Article/details/gzfswybwr.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.fehbvm.com/Article/details/gjlivyfkz.sHtML

find . -mtime -7 -type f
来源：http://read.share.hesvh.cn/Article/details/goiifqkbm.sHtML

[R45] 批量删除
来源：http://www.share.hesvh.cn/Article/details/gkpudsuwa.sHtML

find . -name "*.tmp" -delete
来源：http://blog.hesvh.cn/Article/details/glcpnrxqc.sHtML

[R46] 递归替换文件内容
来源：http://mobile.hesvh.cn/Article/details/goxjpjitw.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.hesvh.cn/Article/details/gdqyijxxm.sHtML

[R47] sed 单行替换
来源：http://wap.fehbvm.com/Article/details/gafqprmkj.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.hesvh.cn/Article/details/gsehtlcfy.sHtML

[R48] awk 取指定列
来源：http://www.blog.zdbjq.cn/Article/details/gtlhlvnpx.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.zdbjq.cn/Article/details/gesomwxoz.sHtML

[R49] awk 带条件
来源：http://m.share.fehbvm.com/Article/details/gtzeplwlm.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.fehbvm.com/Article/details/gebuqcvjh.sHtML

[R50] awk 求和
来源：http://www.blog.fehbvm.com/Article/details/gmkzxfytz.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.fehbvm.com/Article/details/gjphlzisk.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.fehbvm.com/Article/details/grniyyphd.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.zdbjq.cn/Article/details/gtkwctrab.sHtML

[R52] 统计行数
来源：http://m.share.zdbjq.cn/Article/details/gzbhzlcgd.sHtML

wc -l a.txt
来源：http://read.share.fehbvm.com/Article/details/gkldvgete.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.hesvh.cn/Article/details/grslhfenj.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.zdbjq.cn/Article/details/gdnrhamgz.sHtML

[R54] 比较两个文件
来源：http://read.share.fehbvm.com/Article/details/gjslltgbe.sHtML

diff a.txt b.txt
来源：http://mobile.hesvh.cn/Article/details/gjfhvfbhn.sHtML

[R55] 压缩与解压
来源：http://3g.zdbjq.cn/Article/details/gqncsbppk.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.hesvh.cn/Article/details/gbbeybprl.sHtML

[R56] 远程拷贝
来源：http://www.share.zdbjq.cn/Article/details/gvzujcjll.sHtML

scp file user@host:/path/
来源：http://www.m.share.zdbjq.cn/Article/details/gshpkqpkn.sHtML

[R57] 远程执行命令
来源：http://www.m.share.hesvh.cn/Article/details/gqaxydvbu.sHtML

ssh user@host 'uptime'
来源：http://wap.hesvh.cn/Article/details/gitiufcyh.sHtML

[R58] 下载文件
来源：http://www.blog.fehbvm.com/Article/details/gounmpcaf.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.zdbjq.cn/Article/details/gqknvecbu.sHtML

[R59] 发 POST JSON
来源：http://m.share.fehbvm.com/Article/details/ghbscrqry.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.hesvh.cn/Article/details/ggoehyxys.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.hesvh.cn/Article/details/gdkcvtkom.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.hesvh.cn/Article/details/gudctpbxa.sHtML

[R61] 磁盘占用
来源：http://www.m.share.hesvh.cn/Article/details/gonqfitod.sHtML

df -h;  du -sh *
来源：http://read.share.hesvh.cn/Article/details/gwhcpsooa.sHtML

[R62] 找最占空间的文件
来源：http://read.share.hesvh.cn/Article/details/gbcjnevnm.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.fehbvm.com/Article/details/golyldrjk.sHtML

[R63] 内存与进程
来源：http://wap.zdbjq.cn/Article/details/gpynrjcct.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.fehbvm.com/Article/details/gqjzuqvkg.sHtML

[R64] 结束进程
来源：http://www.m.share.hesvh.cn/Article/details/gxanhshcu.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.hesvh.cn/Article/details/glyuxlwyn.sHtML

[R65] 查看端口占用
来源：http://3g.zdbjq.cn/Article/details/gltmrgrjn.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.zdbjq.cn/Article/details/ghpjphwwf.sHtML

[R66] 定时任务
来源：http://m.share.zdbjq.cn/Article/details/gkmtlnqyy.sHtML

crontab -e;  crontab -l
来源：http://baike.zdbjq.cn/Article/details/gceliotcg.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.fehbvm.com/Article/details/ggmwtyato.sHtML

openssl rand -hex 16
来源：http://blog.fehbvm.com/Article/details/glygxraeg.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.fehbvm.com/Article/details/gcqycqaow.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.zdbjq.cn/Article/details/gveehamqv.sHtML

[R69] 生成随机密码
来源：http://mobile.fehbvm.com/Article/details/gjqimkctj.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.fehbvm.com/Article/details/gbulptzcx.sHtML

[R70] 时间戳与互转
来源：http://www.share.zdbjq.cn/Article/details/geynghkbn.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.zdbjq.cn/Article/details/gynibzbph.sHtML

[R71] 日期格式化
来源：http://read.share.zdbjq.cn/Article/details/gvapxmdzs.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://read.share.zdbjq.cn/Article/details/gbucpgumy.sHtML

[R72] 等待端口就绪
来源：http://m.share.hesvh.cn/Article/details/grklxldhx.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.hesvh.cn/Article/details/giqawvdxk.sHtML

[R73] 分割大日志
来源：http://m.share.fehbvm.com/Article/details/gkowierbc.sHtML

split -l 1000 big.log part_
来源：http://baike.fehbvm.com/Article/details/gknyhcjnl.sHtML

[R74] 批量重命名
来源：http://www.blog.fehbvm.com/Article/details/gjapbaqrh.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.fehbvm.com/Article/details/gcmgjbdqi.sHtML

[R75] 导出环境变量
来源：http://www.blog.zdbjq.cn/Article/details/gyttfrnha.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.zdbjq.cn/Article/details/grlywiycc.sHtML

[R76] 使用临时文件
来源：http://baike.hesvh.cn/Article/details/ghwegverm.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.zdbjq.cn/Article/details/gjqjjeaps.sHtML

[R77] 读取用户输入
来源：http://mobile.zdbjq.cn/Article/details/gqufaveav.sHtML

read -rp "请输入: " ans
来源：http://wap.zdbjq.cn/Article/details/gtikkgudj.sHtML

[R78] 交互式菜单
来源：http://m.share.zdbjq.cn/Article/details/gbbvqhcmu.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.fehbvm.com/Article/details/gkoonrieb.sHtML

[R79] 解析命令行选项
来源：http://3g.zdbjq.cn/Article/details/ggbfomxew.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.fehbvm.com/Article/details/gsefmbwtm.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.fehbvm.com/Article/details/ghinsrfqn.sHtML

time ./run.sh
来源：http://mobile.hesvh.cn/Article/details/gvydqzzlg.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/ghwiotowb.sHtML

S. C / C++ 专题
来源：http://baike.fehbvm.com/Article/details/gzisywdar.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gebqywwdn.sHtML

[S01] C：Hello World
来源：http://m.share.hesvh.cn/Article/details/govgkrgxc.sHtML

#include <stdio.h>
来源：http://www.share.fehbvm.com/Article/details/gumcjoglf.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.zdbjq.cn/Article/details/gkafvupjj.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.zdbjq.cn/Article/details/gwhavudcv.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.zdbjq.cn/Article/details/gacuzzyrz.sHtML

[S03] C：读入整数
来源：http://www.share.zdbjq.cn/Article/details/gogfdgotj.sHtML

int x; scanf("%d", &x);
来源：http://www.share.fehbvm.com/Article/details/gjdnhcxea.sHtML

[S04] C：字符串复制
来源：http://mobile.hesvh.cn/Article/details/giimatwcs.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.zdbjq.cn/Article/details/gkuejvfsh.sHtML

[S05] C：字符串长度
来源：http://wap.zdbjq.cn/Article/details/gakoynqhz.sHtML

strlen(s)
来源：http://baike.hesvh.cn/Article/details/gujthojiv.sHtML

[S06] C：字符串比较
来源：http://blog.hesvh.cn/Article/details/gbfktojpe.sHtML

strcmp(a, b) == 0
来源：http://www.blog.hesvh.cn/Article/details/gtdfebeyi.sHtML

[S07] C：数组遍历求和
来源：http://3g.hesvh.cn/Article/details/gnkiutxag.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.zdbjq.cn/Article/details/gttzcffwv.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.hesvh.cn/Article/details/gldxferpy.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.fehbvm.com/Article/details/gkyayvyof.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.fehbvm.com/Article/details/giqevbemy.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.hesvh.cn/Article/details/gspazwpai.sHtML

[S10] C：指针与解引用
来源：http://blog.zdbjq.cn/Article/details/gyocwpdce.sHtML

int *p = &a;  *p = 5;
来源：http://3g.hesvh.cn/Article/details/gerpqlsjr.sHtML

[S11] C：逐行读文件
来源：http://mobile.fehbvm.com/Article/details/gmjionfop.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.zdbjq.cn/Article/details/gqjjxtivi.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.fehbvm.com/Article/details/grrsjxvra.sHtML

fclose(f);
来源：http://www.share.zdbjq.cn/Article/details/guwyxtbon.sHtML

[S12] C：写文件
来源：http://read.share.hesvh.cn/Article/details/gbwjeghye.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.fehbvm.com/Article/details/gslzeuadg.sHtML

[S13] C：宏定义
来源：http://baike.zdbjq.cn/Article/details/gmexsomre.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.zdbjq.cn/Article/details/gttggcuyr.sHtML

[S14] C：枚举
来源：http://mobile.fehbvm.com/Article/details/gmnjekjpd.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.zdbjq.cn/Article/details/gwcqhzlav.sHtML

[S15] C：类型转换
来源：http://baike.zdbjq.cn/Article/details/gawghzpge.sHtML

(double) a / b
来源：http://www.blog.fehbvm.com/Article/details/gpwkhrbxi.sHtML

[S16] C：位操作置位
来源：http://www.blog.fehbvm.com/Article/details/gjavhhtje.sHtML

x |= (1 << 3);
来源：http://baike.hesvh.cn/Article/details/gwzoufseg.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.fehbvm.com/Article/details/gjabwznka.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.hesvh.cn/Article/details/gmesrfqxx.sHtML

[S18] C：命令行参数
来源：http://baike.fehbvm.com/Article/details/gqakdlcpp.sHtML

int main(int argc, char **argv)
来源：http://blog.fehbvm.com/Article/details/gsfjhgudk.sHtML

[S19] C：快速排序
来源：http://www.blog.zdbjq.cn/Article/details/grxfryidk.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.hesvh.cn/Article/details/geaszdsza.sHtML

[S20] C：二分查找
来源：http://read.share.fehbvm.com/Article/details/genpqexii.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.hesvh.cn/Article/details/gwbzajgqc.sHtML

[S21] C：字符类别判断
来源：http://m.share.hesvh.cn/Article/details/guqackouv.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.zdbjq.cn/Article/details/gemtbyuot.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.zdbjq.cn/Article/details/gjqnbucqm.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.zdbjq.cn/Article/details/ghenvjdyp.sHtML

[S23] C：随机数
来源：http://3g.hesvh.cn/Article/details/gfhrrevwr.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.fehbvm.com/Article/details/gfonsakxm.sHtML

[S24] C：获取本地时间
来源：http://m.share.zdbjq.cn/Article/details/gcqnvvkvf.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.hesvh.cn/Article/details/gugxorpye.sHtML

[S25] C：内存拷贝
来源：http://blog.fehbvm.com/Article/details/gpkmmqahs.sHtML

memcpy(dst, src, n);
来源：http://www.blog.fehbvm.com/Article/details/gixnkypwz.sHtML

[S26] C：内存清零
来源：http://baike.fehbvm.com/Article/details/glrqbbtyn.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.hesvh.cn/Article/details/gidnalzva.sHtML

[S27] C：定义常量
来源：http://3g.fehbvm.com/Article/details/gmijsuwts.sHtML

const double PI = 3.14159;
来源：http://read.share.hesvh.cn/Article/details/gpxubijye.sHtML

[S28] C：静态变量
来源：http://read.share.fehbvm.com/Article/details/gbwqslrzq.sHtML

static int counter = 0;
来源：http://blog.zdbjq.cn/Article/details/gbzqhjuho.sHtML

[S29] C：变参函数
来源：http://baike.hesvh.cn/Article/details/goxwisnom.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.fehbvm.com/Article/details/glhlofggi.sHtML

[S30] C：头文件保护
来源：http://blog.hesvh.cn/Article/details/gwyzeoqlf.sHtML

#ifndef X_H
来源：http://www.blog.fehbvm.com/Article/details/grqidixck.sHtML

#define X_H
来源：http://wap.fehbvm.com/Article/details/gbikbtoxa.sHtML

#endif
来源：http://mobile.fehbvm.com/Article/details/gftedaajz.sHtML

[S31] C++：Hello World
来源：http://www.blog.fehbvm.com/Article/details/gqgkqqnjt.sHtML

#include <iostream>
来源：http://www.blog.hesvh.cn/Article/details/gjuqpwqgs.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.zdbjq.cn/Article/details/ggbjegmrz.sHtML

[S32] C++：字符串
来源：http://www.m.share.zdbjq.cn/Article/details/ggqanmxhg.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.zdbjq.cn/Article/details/gtpccuvdi.sHtML

[S33] C++：vector 增删
来源：http://3g.fehbvm.com/Article/details/ghcjdygzy.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.zdbjq.cn/Article/details/goldtuscz.sHtML

[S34] C++：遍历 vector
来源：http://baike.hesvh.cn/Article/details/gsesiljaw.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.fehbvm.com/Article/details/gkmpuvfas.sHtML

[S35] C++：map
来源：http://www.share.zdbjq.cn/Article/details/gitcqzqwh.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fehbvm.com/Article/details/gysdopvlz.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.fehbvm.com/Article/details/gafpvymvz.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.fehbvm.com/Article/details/gicsujnnk.sHtML


<!-- 参考信息 -->