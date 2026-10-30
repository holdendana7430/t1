代发 wailian999

SHOW INDEX FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmudznhfh.sHtML

[Q73] 查看表状态
来源：http://wap.fanxiaobao.xyz/Article/details/ggwpzcfqw.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://blog.fanxiaobao.xyz/Article/details/gcmmfykzu.sHtML

[Q74] 强制使用索引
来源：http://wap.fanxiaobao.xyz/Article/details/gqjvhemgo.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wap.fanxiaobao.xyz/Article/details/gqohoawzm.sHtML

[Q75] 日期格式化
来源：http://3g.fanxiaobao.xyz/Article/details/gvjexogrw.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkdxgssdr.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.fanxiaobao.xyz/Article/details/gaffvgdru.sHtML

[Q76] 按天统计
来源：http://m.share.fanxiaobao.xyz/Article/details/gdkpteqex.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://baike.fanxiaobao.xyz/Article/details/gomzaksss.sHtML

[Q77] 时间加减
来源：http://mobile.fanxiaobao.xyz/Article/details/gnqilwoli.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.share.fanxiaobao.xyz/Article/details/gfymufigp.sHtML

[Q78] 当前时间
来源：http://read.share.fanxiaobao.xyz/Article/details/ggfvyryjv.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wap.fanxiaobao.xyz/Article/details/gntyzcoyd.sHtML

[Q79] 字符串拼接
来源：http://wap.fanxiaobao.xyz/Article/details/gjltmkehs.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goypsdjcg.sHtML

[Q80] 字符串截取
来源：http://mobile.fanxiaobao.xyz/Article/details/gjiasaler.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/guzmzmlii.sHtML

[Q81] 字符串替换
来源：http://www.share.fanxiaobao.xyz/Article/details/gtstbkzum.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/ghljivzrk.sHtML

[Q82] 字符长度与字节长度
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsexjzhbw.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/glbhyttnk.sHtML

[Q83] 大小写转换
来源：http://3g.fanxiaobao.xyz/Article/details/gkudlofai.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gugnrludx.sHtML

[Q84] 去除首尾空格
来源：http://m.share.fanxiaobao.xyz/Article/details/gryixjpco.sHtML

SELECT TRIM(name) FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gosdqeeas.sHtML

[Q85] 数值取整
来源：http://read.share.fanxiaobao.xyz/Article/details/gbjshehls.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://blog.fanxiaobao.xyz/Article/details/gixptcsqs.sHtML

[Q86] 读取 JSON 字段
来源：http://3g.fanxiaobao.xyz/Article/details/gkushkaji.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.fanxiaobao.xyz/Article/details/gqqmmdyyv.sHtML

[Q87] JSON 字段做条件
来源：http://baike.fanxiaobao.xyz/Article/details/gwcipoyhe.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gacknetmw.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpvoyijbu.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://baike.fanxiaobao.xyz/Article/details/gqyeglyap.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gahsikxew.sHtML

[Q89] 判断表是否存在
来源：http://3g.fanxiaobao.xyz/Article/details/gkzyaetgx.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.fanxiaobao.xyz/Article/details/gljpnbuft.sHtML

[Q90] 生成序号列
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmiofaede.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://3g.fanxiaobao.xyz/Article/details/gquemqmwt.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjkvehwry.sHtML

R. Bash 专题
来源：http://wap.fanxiaobao.xyz/Article/details/giqzbjkkv.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gsetjcfop.sHtML

[R01] shebang 与严格模式
来源：http://m.share.fanxiaobao.xyz/Article/details/gbgksrcqv.sHtML

#!/usr/bin/env bash
来源：http://www.blog.fanxiaobao.xyz/Article/details/glbhsuodr.sHtML

set -euo pipefail
来源：http://wap.fanxiaobao.xyz/Article/details/gopacrrrc.sHtML

[R02] 变量赋值与使用
来源：http://www.share.fanxiaobao.xyz/Article/details/ggntpovwj.sHtML

name="Tom"; echo "$name"
来源：http://read.share.fanxiaobao.xyz/Article/details/goggrwvcd.sHtML

[R03] 只读变量
来源：http://3g.fanxiaobao.xyz/Article/details/gohrvnldi.sHtML

readonly PI=3.14
来源：http://3g.fanxiaobao.xyz/Article/details/gqgkhvkdo.sHtML

[R04] 位置参数
来源：http://baike.fanxiaobao.xyz/Article/details/giuniferj.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.fanxiaobao.xyz/Article/details/gczflxbbo.sHtML

[R05] 参数默认值
来源：http://blog.fanxiaobao.xyz/Article/details/glzzhqdoe.sHtML

name="${1:-default}"
来源：http://wap.fanxiaobao.xyz/Article/details/gxdrqirpq.sHtML

[R06] 判断命令是否存在
来源：http://mobile.fanxiaobao.xyz/Article/details/gkgcdtyov.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.fanxiaobao.xyz/Article/details/grzcgjmog.sHtML

[R07] if 判断文件
来源：http://wap.fanxiaobao.xyz/Article/details/glldugoxq.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/gwbwzzpvm.sHtML

[R08] 数值比较
来源：http://mobile.fanxiaobao.xyz/Article/details/gccajcaxd.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://m.share.fanxiaobao.xyz/Article/details/gmfgylhhl.sHtML

[R09] 字符串比较
来源：http://mobile.fanxiaobao.xyz/Article/details/ghldtzefx.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gueceihva.sHtML

[R10] 正则匹配
来源：http://m.share.fanxiaobao.xyz/Article/details/gogljrzkn.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gojirdwux.sHtML

[R11] case 多分支
来源：http://wap.fanxiaobao.xyz/Article/details/gwebrinjq.sHtML

case "$1" in
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmhfremwz.sHtML

start) echo "启动" ;;
来源：http://baike.fanxiaobao.xyz/Article/details/gymtfosaa.sHtML

stop)  echo "停止" ;;
来源：http://3g.fanxiaobao.xyz/Article/details/giblylsne.sHtML

*)     echo "未知命令" ;;
来源：http://blog.fanxiaobao.xyz/Article/details/gbvrgkgvp.sHtML

esac
来源：http://m.share.fanxiaobao.xyz/Article/details/gepwraenn.sHtML

[R12] for 遍历文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gardgtxiu.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.fanxiaobao.xyz/Article/details/gyrkeuvgd.sHtML

[R13] for 计数循环
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqlzeakmn.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gwnhfiafb.sHtML

[R14] C 风格 for
来源：http://read.share.fanxiaobao.xyz/Article/details/gbobzrdnq.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gzwpcgxxf.sHtML

[R15] while 逐行读文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gftbauyvm.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gkycudnbh.sHtML

[R16] until 等待条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gytinzzwd.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.fanxiaobao.xyz/Article/details/ghlxvnxza.sHtML

[R17] 数组定义与取值
来源：http://mobile.fanxiaobao.xyz/Article/details/goybbsphs.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvvvahwum.sHtML

[R18] 遍历数组
来源：http://m.share.fanxiaobao.xyz/Article/details/gjozylcbo.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.fanxiaobao.xyz/Article/details/ghkecosuy.sHtML

[R19] 数组长度
来源：http://blog.fanxiaobao.xyz/Article/details/gypyvjrxe.sHtML

echo "${#arr[@]}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gseijphfx.sHtML

[R20] 关联数组（字典）
来源：http://blog.fanxiaobao.xyz/Article/details/gbnzbbrrn.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggzpqbswk.sHtML

[R21] 字符串长度
来源：http://wap.fanxiaobao.xyz/Article/details/gxhlklmiw.sHtML

echo "${#s}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbndppbpx.sHtML

[R22] 截取子串
来源：http://www.share.fanxiaobao.xyz/Article/details/giyoobgny.sHtML

echo "${s:0:5}"
来源：http://3g.fanxiaobao.xyz/Article/details/gzlrrueqw.sHtML

[R23] 字符串替换
来源：http://3g.fanxiaobao.xyz/Article/details/gslxvamhg.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.fanxiaobao.xyz/Article/details/grcwwrfvj.sHtML

[R24] 大小写转换
来源：http://www.share.fanxiaobao.xyz/Article/details/gyvqjxqkp.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.fanxiaobao.xyz/Article/details/gvmowxxmv.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.fanxiaobao.xyz/Article/details/gyzqfafry.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gxcfgbmeo.sHtML

[R26] 命令替换
来源：http://3g.fanxiaobao.xyz/Article/details/gpdcgoklk.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.fanxiaobao.xyz/Article/details/gutplghhi.sHtML

[R27] 算术展开
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjetknnbu.sHtML

echo $((1 + 2 * 3))
来源：http://baike.fanxiaobao.xyz/Article/details/guvazdkeu.sHtML

[R28] 浮点运算
来源：http://wap.fanxiaobao.xyz/Article/details/gszijzuza.sHtML

echo "scale=2; 10/3" | bc
来源：http://m.share.fanxiaobao.xyz/Article/details/gneehkqbe.sHtML

[R29] 定义函数
来源：http://read.share.fanxiaobao.xyz/Article/details/glpdlvvcb.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.fanxiaobao.xyz/Article/details/gjodfeqxc.sHtML

[R30] 函数返回状态码
来源：http://wap.fanxiaobao.xyz/Article/details/gsmfczrqn.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghtwutght.sHtML

[R31] 局部变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gxrvppzno.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.fanxiaobao.xyz/Article/details/gstijzrej.sHtML

[R32] 参数个数校验
来源：http://www.share.fanxiaobao.xyz/Article/details/grcospuud.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gjtixwsli.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.fanxiaobao.xyz/Article/details/gscqtxuan.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.fanxiaobao.xyz/Article/details/grvlaayqr.sHtML

[R34] 退出时清理
来源：http://blog.fanxiaobao.xyz/Article/details/gpgpijzsx.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.fanxiaobao.xyz/Article/details/gackotifk.sHtML

[R35] 后台执行并等待
来源：http://www.blog.fanxiaobao.xyz/Article/details/glqzfcrdh.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://3g.fanxiaobao.xyz/Article/details/gdafcztlb.sHtML

[R36] 并发执行多个任务
来源：http://mobile.fanxiaobao.xyz/Article/details/gsoobyrxf.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.fanxiaobao.xyz/Article/details/gjegjspxo.sHtML

[R37] 把输出赋给变量
来源：http://3g.fanxiaobao.xyz/Article/details/gjhenxkmm.sHtML

files=$(ls -1)
来源：http://wap.fanxiaobao.xyz/Article/details/giawezuyj.sHtML

[R38] 管道串联
来源：http://blog.fanxiaobao.xyz/Article/details/garzlcggp.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.fanxiaobao.xyz/Article/details/gzbanmhkw.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.fanxiaobao.xyz/Article/details/gynmtpjlo.sHtML

cmd > out.log 2>&1
来源：http://mobile.fanxiaobao.xyz/Article/details/gslptomjm.sHtML

[R40] 追加写日志
来源：http://wap.fanxiaobao.xyz/Article/details/guthepwqr.sHtML

echo "log" >> out.log
来源：http://3g.fanxiaobao.xyz/Article/details/gjrhlbloq.sHtML

[R41] 丢弃输出
来源：http://3g.fanxiaobao.xyz/Article/details/gysxmeepu.sHtML

cmd >/dev/null 2>&1
来源：http://blog.fanxiaobao.xyz/Article/details/geufxblzo.sHtML

[R42] 输入重定向
来源：http://baike.fanxiaobao.xyz/Article/details/gyabkevvk.sHtML

wc -l < a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gbgpbbfug.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaotbkqtm.sHtML

find . -name "*.log" -type f
来源：http://blog.fanxiaobao.xyz/Article/details/gwnqselvv.sHtML

[R44] 按修改时间查找
来源：http://mobile.fanxiaobao.xyz/Article/details/gzrksrnta.sHtML

find . -mtime -7 -type f
来源：http://www.share.fanxiaobao.xyz/Article/details/gvukfhfis.sHtML

[R45] 批量删除
来源：http://baike.fanxiaobao.xyz/Article/details/gzdtidpkk.sHtML

find . -name "*.tmp" -delete
来源：http://blog.fanxiaobao.xyz/Article/details/ghjhygsas.sHtML

[R46] 递归替换文件内容
来源：http://blog.fanxiaobao.xyz/Article/details/gpyqghafj.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.fanxiaobao.xyz/Article/details/gszbwvpem.sHtML

[R47] sed 单行替换
来源：http://blog.fanxiaobao.xyz/Article/details/gszmtshga.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gyqlbfckh.sHtML

[R48] awk 取指定列
来源：http://3g.fanxiaobao.xyz/Article/details/geqyoatlg.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gnlauajpx.sHtML

[R49] awk 带条件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvxckganz.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.fanxiaobao.xyz/Article/details/goiyiilzf.sHtML

[R50] awk 求和
来源：http://blog.fanxiaobao.xyz/Article/details/geastdkyd.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gfttofmxp.sHtML

[R51] 排序去重取前几
来源：http://blog.fanxiaobao.xyz/Article/details/gaaruadzn.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcmtbdjta.sHtML

[R52] 统计行数
来源：http://www.share.fanxiaobao.xyz/Article/details/goucfxtag.sHtML

wc -l a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwdenrzss.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.fanxiaobao.xyz/Article/details/gokeiddti.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.fanxiaobao.xyz/Article/details/glfubholc.sHtML

[R54] 比较两个文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gadkcwozj.sHtML

diff a.txt b.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gydzxaenm.sHtML

[R55] 压缩与解压
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmexqzdax.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.fanxiaobao.xyz/Article/details/gisfszgmg.sHtML

[R56] 远程拷贝
来源：http://read.share.fanxiaobao.xyz/Article/details/gtcrfcbsp.sHtML

scp file user@host:/path/
来源：http://www.share.fanxiaobao.xyz/Article/details/ggygdfpjn.sHtML

[R57] 远程执行命令
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gopkqfheg.sHtML

ssh user@host 'uptime'
来源：http://mobile.fanxiaobao.xyz/Article/details/givebtvjk.sHtML

[R58] 下载文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gfdwrjqap.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbwahnogk.sHtML

[R59] 发 POST JSON
来源：http://3g.fanxiaobao.xyz/Article/details/gpkwymnkz.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxlocjyvz.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.fanxiaobao.xyz/Article/details/gszeecope.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.fanxiaobao.xyz/Article/details/gcfjkmigq.sHtML

[R61] 磁盘占用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkdrfrpic.sHtML

df -h;  du -sh *
来源：http://wap.fanxiaobao.xyz/Article/details/gglqhofeo.sHtML

[R62] 找最占空间的文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gmgokgcua.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.fanxiaobao.xyz/Article/details/gupzmqoei.sHtML

[R63] 内存与进程
来源：http://m.share.fanxiaobao.xyz/Article/details/gmgpmwbdi.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.fanxiaobao.xyz/Article/details/gzjhfjfbi.sHtML

[R64] 结束进程
来源：http://read.share.fanxiaobao.xyz/Article/details/guybnoftu.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gistjxsnx.sHtML

[R65] 查看端口占用
来源：http://m.share.fanxiaobao.xyz/Article/details/gcedeoocv.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggqcrpisp.sHtML

[R66] 定时任务
来源：http://blog.fanxiaobao.xyz/Article/details/gnytxdfjo.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.fanxiaobao.xyz/Article/details/getkicxra.sHtML

[R67] 生成随机十六进制串
来源：http://baike.fanxiaobao.xyz/Article/details/gugrcwfpm.sHtML

openssl rand -hex 16
来源：http://read.share.fanxiaobao.xyz/Article/details/gvvhwgtgj.sHtML

[R68] 计算文件校验值
来源：http://m.share.fanxiaobao.xyz/Article/details/gwvssdosi.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gcxdsfsyj.sHtML

[R69] 生成随机密码
来源：http://mobile.fanxiaobao.xyz/Article/details/gfholrfjx.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.fanxiaobao.xyz/Article/details/gnwxozner.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjjjzeggd.sHtML

date +%s;  date -d @1700000000
来源：http://wap.fanxiaobao.xyz/Article/details/gzqeqqrcm.sHtML

[R71] 日期格式化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjxkgqivm.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.fanxiaobao.xyz/Article/details/grrucidsw.sHtML

[R72] 等待端口就绪
来源：http://mobile.fanxiaobao.xyz/Article/details/giyuvmbcn.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.fanxiaobao.xyz/Article/details/ghqhwgqca.sHtML

[R73] 分割大日志
来源：http://3g.fanxiaobao.xyz/Article/details/glthgqqob.sHtML

split -l 1000 big.log part_
来源：http://www.share.fanxiaobao.xyz/Article/details/gtigszjic.sHtML

[R74] 批量重命名
来源：http://read.share.fanxiaobao.xyz/Article/details/gqstykoqc.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.fanxiaobao.xyz/Article/details/giphklbkr.sHtML

[R75] 导出环境变量
来源：http://baike.fanxiaobao.xyz/Article/details/gdtqcrkgf.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.fanxiaobao.xyz/Article/details/gezwgrqle.sHtML

[R76] 使用临时文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gollrzvfq.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fanxiaobao.xyz/Article/details/gagnkqeyt.sHtML

[R77] 读取用户输入
来源：http://blog.fanxiaobao.xyz/Article/details/ghuedsodb.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmjjueekf.sHtML

[R78] 交互式菜单
来源：http://blog.fanxiaobao.xyz/Article/details/gzkhgadkf.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.fanxiaobao.xyz/Article/details/gljxpiudu.sHtML

[R79] 解析命令行选项
来源：http://www.share.fanxiaobao.xyz/Article/details/gkearucfd.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.fanxiaobao.xyz/Article/details/gtocxooen.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqkchrfgl.sHtML

time ./run.sh
来源：http://wap.fanxiaobao.xyz/Article/details/garhznwfr.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gwmpqgyvd.sHtML

S. C / C++ 专题
来源：http://www.share.fanxiaobao.xyz/Article/details/gotfqkdcw.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/ghcayxpri.sHtML

[S01] C：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdycozazw.sHtML

#include <stdio.h>
来源：http://www.share.fanxiaobao.xyz/Article/details/gllpqygot.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.fanxiaobao.xyz/Article/details/gpmxfobir.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.fanxiaobao.xyz/Article/details/guavlmskw.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjavkttwb.sHtML

[S03] C：读入整数
来源：http://read.share.fanxiaobao.xyz/Article/details/gcecntmab.sHtML

int x; scanf("%d", &x);
来源：http://m.share.fanxiaobao.xyz/Article/details/gpibpasee.sHtML

[S04] C：字符串复制
来源：http://m.share.fanxiaobao.xyz/Article/details/gxxqkbema.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.fanxiaobao.xyz/Article/details/gstgzoqrd.sHtML

[S05] C：字符串长度
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxqnamkvz.sHtML

strlen(s)
来源：http://baike.fanxiaobao.xyz/Article/details/gynemmytu.sHtML

[S06] C：字符串比较
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdryziudo.sHtML

strcmp(a, b) == 0
来源：http://read.share.fanxiaobao.xyz/Article/details/gtugizutg.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwthzcuxt.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.fanxiaobao.xyz/Article/details/gguiwxsvi.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.fanxiaobao.xyz/Article/details/gnygjdnoj.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.fanxiaobao.xyz/Article/details/gtqqjljxd.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.fanxiaobao.xyz/Article/details/gnjmkbsbn.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.fanxiaobao.xyz/Article/details/grntlcarv.sHtML

[S10] C：指针与解引用
来源：http://mobile.fanxiaobao.xyz/Article/details/givxkkteo.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdyphohls.sHtML

[S11] C：逐行读文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gpgzeovbu.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.fanxiaobao.xyz/Article/details/gytrxzplf.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkzwsejtb.sHtML

fclose(f);
来源：http://wap.fanxiaobao.xyz/Article/details/gvkhstafx.sHtML

[S12] C：写文件
来源：http://3g.fanxiaobao.xyz/Article/details/gkqsonjcd.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.fanxiaobao.xyz/Article/details/gqbhjfodn.sHtML

[S13] C：宏定义
来源：http://www.blog.fanxiaobao.xyz/Article/details/gahqbwglr.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.fanxiaobao.xyz/Article/details/gesejpmkh.sHtML

[S14] C：枚举
来源：http://m.share.fanxiaobao.xyz/Article/details/gbdublswj.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.fanxiaobao.xyz/Article/details/gvpcfaapa.sHtML

[S15] C：类型转换
来源：http://3g.fanxiaobao.xyz/Article/details/gzawuymzk.sHtML

(double) a / b
来源：http://read.share.fanxiaobao.xyz/Article/details/gzoiooqnq.sHtML

[S16] C：位操作置位
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gluafivqo.sHtML

x |= (1 << 3);
来源：http://3g.fanxiaobao.xyz/Article/details/gmgbbqart.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.fanxiaobao.xyz/Article/details/gcjwvrebf.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.fanxiaobao.xyz/Article/details/guxriuthu.sHtML

[S18] C：命令行参数
来源：http://m.share.fanxiaobao.xyz/Article/details/gwnlrlrfs.sHtML

int main(int argc, char **argv)
来源：http://m.share.fanxiaobao.xyz/Article/details/guschsrpe.sHtML

[S19] C：快速排序
来源：http://wap.fanxiaobao.xyz/Article/details/gruygtmnl.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.fanxiaobao.xyz/Article/details/gaowziljk.sHtML

[S20] C：二分查找
来源：http://mobile.fanxiaobao.xyz/Article/details/gqjbugvvv.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.fanxiaobao.xyz/Article/details/gtpyslrug.sHtML

[S21] C：字符类别判断
来源：http://read.share.fanxiaobao.xyz/Article/details/gtkcqvwms.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.fanxiaobao.xyz/Article/details/gcvnqmdoh.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvpqdslmi.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.fanxiaobao.xyz/Article/details/gimxpthhg.sHtML

[S23] C：随机数
来源：http://baike.fanxiaobao.xyz/Article/details/gberhiyhp.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.fanxiaobao.xyz/Article/details/gycwveyfv.sHtML

[S24] C：获取本地时间
来源：http://3g.fanxiaobao.xyz/Article/details/gimgyxpfi.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.fanxiaobao.xyz/Article/details/grragomzv.sHtML

[S25] C：内存拷贝
来源：http://3g.fanxiaobao.xyz/Article/details/gouoxxbyy.sHtML

memcpy(dst, src, n);
来源：http://blog.fanxiaobao.xyz/Article/details/gylbhrrbl.sHtML

[S26] C：内存清零
来源：http://baike.fanxiaobao.xyz/Article/details/grskivtgl.sHtML

memset(a, 0, sizeof a);
来源：http://blog.fanxiaobao.xyz/Article/details/gtecdodei.sHtML

[S27] C：定义常量
来源：http://blog.fanxiaobao.xyz/Article/details/gcqrwtiru.sHtML

const double PI = 3.14159;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkqbobvmu.sHtML

[S28] C：静态变量
来源：http://read.share.fanxiaobao.xyz/Article/details/ghnrsrfmk.sHtML

static int counter = 0;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfcpybyrl.sHtML

[S29] C：变参函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gwlvuahuk.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.fanxiaobao.xyz/Article/details/ggyhxogyl.sHtML

[S30] C：头文件保护
来源：http://www.share.fanxiaobao.xyz/Article/details/geqzplfji.sHtML

#ifndef X_H
来源：http://3g.fanxiaobao.xyz/Article/details/gctlthqgq.sHtML

#define X_H
来源：http://www.share.fanxiaobao.xyz/Article/details/gtghbvrsh.sHtML

#endif
来源：http://3g.fanxiaobao.xyz/Article/details/gipubtvke.sHtML

[S31] C++：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gvheiyzwp.sHtML

#include <iostream>
来源：http://baike.fanxiaobao.xyz/Article/details/gohjwwkkp.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gukfuozja.sHtML

[S32] C++：字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghppdybdi.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.fanxiaobao.xyz/Article/details/goiguqyxm.sHtML

[S33] C++：vector 增删
来源：http://m.share.fanxiaobao.xyz/Article/details/goprvlyzq.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.fanxiaobao.xyz/Article/details/gxjsdlefu.sHtML

[S34] C++：遍历 vector
来源：http://blog.fanxiaobao.xyz/Article/details/gsvymxhuu.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gxztolcbk.sHtML

[S35] C++：map
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqyvwwrgb.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gmkwsilmf.sHtML

[S36] C++：unordered_map
来源：http://blog.fanxiaobao.xyz/Article/details/gmitizdng.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gtyakjvld.sHtML

[S37] C++：set
来源：http://baike.fanxiaobao.xyz/Article/details/gfnrvhasf.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.fanxiaobao.xyz/Article/details/gpmzzrfsb.sHtML

[S38] C++：排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gofrxknbw.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.fanxiaobao.xyz/Article/details/goejfvoej.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghbxxlmvf.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.fanxiaobao.xyz/Article/details/ghkyhwvvk.sHtML

[S40] C++：查找元素
来源：http://wap.fanxiaobao.xyz/Article/details/golfmkaha.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.fanxiaobao.xyz/Article/details/gmyndjhlw.sHtML

[S41] C++：类与构造函数
来源：http://www.share.fanxiaobao.xyz/Article/details/giouwntpc.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.fanxiaobao.xyz/Article/details/gzxzfsewb.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggyfmlprq.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.fanxiaobao.xyz/Article/details/gnbaxbowr.sHtML


<!-- 参考信息 -->