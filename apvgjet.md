代发 wailian999

[Q80] 字符串截取
来源：http://baike.fanxiaobao.xyz/Article/details/gprcciqct.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gjgbrkejg.sHtML

[Q81] 字符串替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gbjrmrkyn.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gqndxtuqb.sHtML

[Q82] 字符长度与字节长度
来源：http://3g.fanxiaobao.xyz/Article/details/gcutmstpu.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gpfxyywou.sHtML

[Q83] 大小写转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpfhyhrbn.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gfmoabqdh.sHtML

[Q84] 去除首尾空格
来源：http://wap.fanxiaobao.xyz/Article/details/gegkxkjac.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gunznrzzh.sHtML

[Q85] 数值取整
来源：http://3g.fanxiaobao.xyz/Article/details/ghbbcwykg.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gruqhdpjr.sHtML

[Q86] 读取 JSON 字段
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaqcfheqe.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.fanxiaobao.xyz/Article/details/ghrbqgqxl.sHtML

[Q87] JSON 字段做条件
来源：http://wap.fanxiaobao.xyz/Article/details/gqhuxzpht.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wap.fanxiaobao.xyz/Article/details/gevesiywy.sHtML

[Q88] 行转列（条件聚合）
来源：http://m.share.fanxiaobao.xyz/Article/details/gjpgxmdmo.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.fanxiaobao.xyz/Article/details/gasuymtmh.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gofwcegpz.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghtniffce.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.fanxiaobao.xyz/Article/details/ghztzsygv.sHtML

[Q90] 生成序号列
来源：http://wap.fanxiaobao.xyz/Article/details/gmwyqmlcl.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://read.share.fanxiaobao.xyz/Article/details/gmyhkrdli.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gnpqwftox.sHtML

R. Bash 专题
来源：http://3g.fanxiaobao.xyz/Article/details/gazeylybi.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjvgwgjpz.sHtML

[R01] shebang 与严格模式
来源：http://wap.fanxiaobao.xyz/Article/details/grbiuanbb.sHtML

#!/usr/bin/env bash
来源：http://blog.fanxiaobao.xyz/Article/details/glyxqtpyo.sHtML

set -euo pipefail
来源：http://www.share.fanxiaobao.xyz/Article/details/gvdkjtvle.sHtML

[R02] 变量赋值与使用
来源：http://3g.fanxiaobao.xyz/Article/details/gbtluwlmt.sHtML

name="Tom"; echo "$name"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/graovfemp.sHtML

[R03] 只读变量
来源：http://read.share.fanxiaobao.xyz/Article/details/grflxnjmp.sHtML

readonly PI=3.14
来源：http://baike.fanxiaobao.xyz/Article/details/gpuktgphl.sHtML

[R04] 位置参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfuycnwst.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.fanxiaobao.xyz/Article/details/gzhwnrojx.sHtML

[R05] 参数默认值
来源：http://wap.fanxiaobao.xyz/Article/details/gyequqozz.sHtML

name="${1:-default}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gebedamqa.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkofzxcqh.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gotxdlmyn.sHtML

[R07] if 判断文件
来源：http://wap.fanxiaobao.xyz/Article/details/giizdofoz.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/gdsseugai.sHtML

[R08] 数值比较
来源：http://3g.fanxiaobao.xyz/Article/details/gkworjbtl.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://mobile.fanxiaobao.xyz/Article/details/gifmpdcla.sHtML

[R09] 字符串比较
来源：http://m.share.fanxiaobao.xyz/Article/details/geizkdxtg.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.fanxiaobao.xyz/Article/details/gxuwthpor.sHtML

[R10] 正则匹配
来源：http://wap.fanxiaobao.xyz/Article/details/giunciryp.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpajgrcdc.sHtML

[R11] case 多分支
来源：http://www.share.fanxiaobao.xyz/Article/details/gdngxzgse.sHtML

case "$1" in
来源：http://wap.fanxiaobao.xyz/Article/details/gdavymcxl.sHtML

start) echo "启动" ;;
来源：http://wap.fanxiaobao.xyz/Article/details/gefivpavw.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gasunbrdu.sHtML

*)     echo "未知命令" ;;
来源：http://www.share.fanxiaobao.xyz/Article/details/gegeyfebe.sHtML

esac
来源：http://mobile.fanxiaobao.xyz/Article/details/gdjjfwedf.sHtML

[R12] for 遍历文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnrllyhqx.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtthxaktn.sHtML

[R13] for 计数循环
来源：http://baike.fanxiaobao.xyz/Article/details/gatpagwom.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gzxzjtpzf.sHtML

[R14] C 风格 for
来源：http://www.share.fanxiaobao.xyz/Article/details/gzchpadav.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.fanxiaobao.xyz/Article/details/geopnnbkn.sHtML

[R15] while 逐行读文件
来源：http://baike.fanxiaobao.xyz/Article/details/gjteyxjak.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gcoeabhcx.sHtML

[R16] until 等待条件
来源：http://blog.fanxiaobao.xyz/Article/details/gosswignj.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.fanxiaobao.xyz/Article/details/gzboapjxt.sHtML

[R17] 数组定义与取值
来源：http://3g.fanxiaobao.xyz/Article/details/gctfqmwsw.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gpzcjtdmd.sHtML

[R18] 遍历数组
来源：http://wap.fanxiaobao.xyz/Article/details/gpwiqnqdy.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.fanxiaobao.xyz/Article/details/guawcpttk.sHtML

[R19] 数组长度
来源：http://blog.fanxiaobao.xyz/Article/details/gdzpfctsf.sHtML

echo "${#arr[@]}"
来源：http://www.share.fanxiaobao.xyz/Article/details/ggcvfiuhv.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gflhdbxtm.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.fanxiaobao.xyz/Article/details/gjboeefbv.sHtML

[R21] 字符串长度
来源：http://wap.fanxiaobao.xyz/Article/details/gcwehebfa.sHtML

echo "${#s}"
来源：http://3g.fanxiaobao.xyz/Article/details/grlbbzpql.sHtML

[R22] 截取子串
来源：http://mobile.fanxiaobao.xyz/Article/details/gqrohgnws.sHtML

echo "${s:0:5}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gglqzqznd.sHtML

[R23] 字符串替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gnknaudwg.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gbwffpaej.sHtML

[R24] 大小写转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdipyqbwg.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gpzbkdfdp.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.fanxiaobao.xyz/Article/details/glrghghgg.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gudjdccpk.sHtML

[R26] 命令替换
来源：http://wap.fanxiaobao.xyz/Article/details/gxejvdprd.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvymksgos.sHtML

[R27] 算术展开
来源：http://mobile.fanxiaobao.xyz/Article/details/gmfopvfnh.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.fanxiaobao.xyz/Article/details/gjzsfgmhy.sHtML

[R28] 浮点运算
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqionemva.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.fanxiaobao.xyz/Article/details/gbzztoool.sHtML

[R29] 定义函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gcmyxbhrs.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.fanxiaobao.xyz/Article/details/ggvxazgfu.sHtML

[R30] 函数返回状态码
来源：http://read.share.fanxiaobao.xyz/Article/details/glugdogcp.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gagaqbglf.sHtML

[R31] 局部变量
来源：http://baike.fanxiaobao.xyz/Article/details/ggdtztton.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gfofecsuc.sHtML

[R32] 参数个数校验
来源：http://m.share.fanxiaobao.xyz/Article/details/gwqczaioh.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gomuiuddt.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.fanxiaobao.xyz/Article/details/gnjrbyxrz.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.fanxiaobao.xyz/Article/details/gxrmiavon.sHtML

[R34] 退出时清理
来源：http://wap.fanxiaobao.xyz/Article/details/gehmondjz.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.fanxiaobao.xyz/Article/details/gxipilfku.sHtML

[R35] 后台执行并等待
来源：http://read.share.fanxiaobao.xyz/Article/details/gtwdzcmve.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.fanxiaobao.xyz/Article/details/guyfcictz.sHtML

[R36] 并发执行多个任务
来源：http://read.share.fanxiaobao.xyz/Article/details/gjuxuksqb.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gapdqickm.sHtML

[R37] 把输出赋给变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gevsyvsho.sHtML

files=$(ls -1)
来源：http://baike.fanxiaobao.xyz/Article/details/gqqlnrrxi.sHtML

[R38] 管道串联
来源：http://3g.fanxiaobao.xyz/Article/details/gfvrrrmlt.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.fanxiaobao.xyz/Article/details/gmcdlkira.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.fanxiaobao.xyz/Article/details/gwwocwnsz.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjvivutdq.sHtML

[R40] 追加写日志
来源：http://blog.fanxiaobao.xyz/Article/details/gizurzmzy.sHtML

echo "log" >> out.log
来源：http://www.blog.fanxiaobao.xyz/Article/details/gslvizgmk.sHtML

[R41] 丢弃输出
来源：http://read.share.fanxiaobao.xyz/Article/details/gqxreqovk.sHtML

cmd >/dev/null 2>&1
来源：http://baike.fanxiaobao.xyz/Article/details/geybpnvgh.sHtML

[R42] 输入重定向
来源：http://read.share.fanxiaobao.xyz/Article/details/gwwqgpedf.sHtML

wc -l < a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyzhlheet.sHtML

[R43] 按名字查找文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gaxumllgh.sHtML

find . -name "*.log" -type f
来源：http://read.share.fanxiaobao.xyz/Article/details/gevcosnfd.sHtML

[R44] 按修改时间查找
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcodeadvf.sHtML

find . -mtime -7 -type f
来源：http://www.share.fanxiaobao.xyz/Article/details/gxhsztcmt.sHtML

[R45] 批量删除
来源：http://blog.fanxiaobao.xyz/Article/details/gklkvwgsj.sHtML

find . -name "*.tmp" -delete
来源：http://baike.fanxiaobao.xyz/Article/details/gfaqlsgka.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.fanxiaobao.xyz/Article/details/grscpukbr.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.fanxiaobao.xyz/Article/details/ggovebcdy.sHtML

[R47] sed 单行替换
来源：http://3g.fanxiaobao.xyz/Article/details/gdycjyibj.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzvimpwig.sHtML

[R48] awk 取指定列
来源：http://3g.fanxiaobao.xyz/Article/details/gqcytefke.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gzqtsjpgm.sHtML

[R49] awk 带条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gazianuly.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.fanxiaobao.xyz/Article/details/ghtffipen.sHtML

[R50] awk 求和
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcoiqmewb.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gfehjkzuq.sHtML

[R51] 排序去重取前几
来源：http://read.share.fanxiaobao.xyz/Article/details/gqokgrixp.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.fanxiaobao.xyz/Article/details/gmosefaeo.sHtML

[R52] 统计行数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkiuskytv.sHtML

wc -l a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gkagtesbc.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.fanxiaobao.xyz/Article/details/gcabpfgvf.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.fanxiaobao.xyz/Article/details/gfbzylkeb.sHtML

[R54] 比较两个文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gtyaicerm.sHtML

diff a.txt b.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gbzimjeby.sHtML

[R55] 压缩与解压
来源：http://read.share.fanxiaobao.xyz/Article/details/gelnapwbn.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvbslycyl.sHtML

[R56] 远程拷贝
来源：http://mobile.fanxiaobao.xyz/Article/details/ggkxqgrgy.sHtML

scp file user@host:/path/
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqukhwtfl.sHtML

[R57] 远程执行命令
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtnkauiyx.sHtML

ssh user@host 'uptime'
来源：http://blog.fanxiaobao.xyz/Article/details/gaxksouiq.sHtML

[R58] 下载文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfozqjhob.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.fanxiaobao.xyz/Article/details/glitgivgg.sHtML

[R59] 发 POST JSON
来源：http://baike.fanxiaobao.xyz/Article/details/gfhqqeelv.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjbxgxogl.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.fanxiaobao.xyz/Article/details/gkwevrzin.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.fanxiaobao.xyz/Article/details/ggmjoawlq.sHtML

[R61] 磁盘占用
来源：http://www.share.fanxiaobao.xyz/Article/details/gxrpxzpwt.sHtML

df -h;  du -sh *
来源：http://www.share.fanxiaobao.xyz/Article/details/gmnfgwaah.sHtML

[R62] 找最占空间的文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gzzkpislc.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcblhvahs.sHtML

[R63] 内存与进程
来源：http://www.share.fanxiaobao.xyz/Article/details/glotyxodo.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.fanxiaobao.xyz/Article/details/gzqrwurdp.sHtML

[R64] 结束进程
来源：http://baike.fanxiaobao.xyz/Article/details/gkpzkqpxs.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.fanxiaobao.xyz/Article/details/gtwvqvywh.sHtML

[R65] 查看端口占用
来源：http://m.share.fanxiaobao.xyz/Article/details/gpqosytnj.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.fanxiaobao.xyz/Article/details/gbmxeplbb.sHtML

[R66] 定时任务
来源：http://baike.fanxiaobao.xyz/Article/details/gxbieddbv.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtxcwebtr.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.fanxiaobao.xyz/Article/details/ghuultfhy.sHtML

openssl rand -hex 16
来源：http://www.blog.fanxiaobao.xyz/Article/details/gohrdnphc.sHtML

[R68] 计算文件校验值
来源：http://mobile.fanxiaobao.xyz/Article/details/gieknsdso.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/giwpskfqb.sHtML

[R69] 生成随机密码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guzleiqpc.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.fanxiaobao.xyz/Article/details/gflaysgkc.sHtML

[R70] 时间戳与互转
来源：http://blog.fanxiaobao.xyz/Article/details/gzmfkldzk.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.fanxiaobao.xyz/Article/details/gudxjlthl.sHtML

[R71] 日期格式化
来源：http://wap.fanxiaobao.xyz/Article/details/gqjxysywc.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.fanxiaobao.xyz/Article/details/gquzfugsb.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxsuzxhyt.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjtzrbtwn.sHtML

[R73] 分割大日志
来源：http://read.share.fanxiaobao.xyz/Article/details/gafpldunx.sHtML

split -l 1000 big.log part_
来源：http://www.share.fanxiaobao.xyz/Article/details/gqnwqpzxm.sHtML

[R74] 批量重命名
来源：http://www.share.fanxiaobao.xyz/Article/details/gcciwvhmz.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxvpmfkkj.sHtML

[R75] 导出环境变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtckhxnfp.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gczwsnxyc.sHtML

[R76] 使用临时文件
来源：http://baike.fanxiaobao.xyz/Article/details/gzbjnthod.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goblblbcy.sHtML

[R77] 读取用户输入
来源：http://www.share.fanxiaobao.xyz/Article/details/gftyxipyv.sHtML

read -rp "请输入: " ans
来源：http://3g.fanxiaobao.xyz/Article/details/gxonaebrs.sHtML

[R78] 交互式菜单
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfgdlisku.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.fanxiaobao.xyz/Article/details/guvckdwib.sHtML

[R79] 解析命令行选项
来源：http://baike.fanxiaobao.xyz/Article/details/gbwnhvxnu.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gdlmwdrrd.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.fanxiaobao.xyz/Article/details/ggaubbqhq.sHtML

time ./run.sh
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggprcdvip.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gcxpfcetg.sHtML

S. C / C++ 专题
来源：http://mobile.fanxiaobao.xyz/Article/details/grdnobszv.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gynteortr.sHtML

[S01] C：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gjhpntogb.sHtML

#include <stdio.h>
来源：http://baike.fanxiaobao.xyz/Article/details/gyasalcek.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghycqikwx.sHtML

[S02] C：变量与格式化输出
来源：http://wap.fanxiaobao.xyz/Article/details/gkrmhaaik.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.fanxiaobao.xyz/Article/details/gyqklmcsx.sHtML

[S03] C：读入整数
来源：http://www.share.fanxiaobao.xyz/Article/details/gbdxcpcfl.sHtML

int x; scanf("%d", &x);
来源：http://baike.fanxiaobao.xyz/Article/details/gsgehxlbd.sHtML

[S04] C：字符串复制
来源：http://3g.fanxiaobao.xyz/Article/details/gqaznakvp.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.fanxiaobao.xyz/Article/details/gqumoyule.sHtML

[S05] C：字符串长度
来源：http://www.share.fanxiaobao.xyz/Article/details/gufqbfyjq.sHtML

strlen(s)
来源：http://blog.fanxiaobao.xyz/Article/details/gnavqfkbu.sHtML

[S06] C：字符串比较
来源：http://baike.fanxiaobao.xyz/Article/details/gduuabhyk.sHtML

strcmp(a, b) == 0
来源：http://3g.fanxiaobao.xyz/Article/details/gefkpuqjx.sHtML

[S07] C：数组遍历求和
来源：http://baike.fanxiaobao.xyz/Article/details/gvbgjdwiq.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.fanxiaobao.xyz/Article/details/gqsormhly.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.fanxiaobao.xyz/Article/details/gsnygbtfl.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grqcbohug.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.fanxiaobao.xyz/Article/details/gjwyniokr.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.fanxiaobao.xyz/Article/details/gplbwttmn.sHtML

[S10] C：指针与解引用
来源：http://m.share.fanxiaobao.xyz/Article/details/gxwjrkivy.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.fanxiaobao.xyz/Article/details/gwptulknh.sHtML

[S11] C：逐行读文件
来源：http://blog.fanxiaobao.xyz/Article/details/gtomgdlyi.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.fanxiaobao.xyz/Article/details/gydnttdid.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.fanxiaobao.xyz/Article/details/gibrxnmni.sHtML

fclose(f);
来源：http://www.share.fanxiaobao.xyz/Article/details/gzdygntcp.sHtML

[S12] C：写文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gcehlhmfn.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpxnscmsx.sHtML

[S13] C：宏定义
来源：http://mobile.fanxiaobao.xyz/Article/details/gmhuixkqv.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.fanxiaobao.xyz/Article/details/gmttjwykg.sHtML

[S14] C：枚举
来源：http://www.share.fanxiaobao.xyz/Article/details/grzaxvihm.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.fanxiaobao.xyz/Article/details/gummxxmli.sHtML

[S15] C：类型转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtzodsima.sHtML

(double) a / b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghowgocbv.sHtML

[S16] C：位操作置位
来源：http://read.share.fanxiaobao.xyz/Article/details/gdrhwhoie.sHtML

x |= (1 << 3);
来源：http://wap.fanxiaobao.xyz/Article/details/gefuxuhzr.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.fanxiaobao.xyz/Article/details/gqiwhsivl.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.fanxiaobao.xyz/Article/details/gxxzcngib.sHtML

[S18] C：命令行参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcotihqro.sHtML

int main(int argc, char **argv)
来源：http://3g.fanxiaobao.xyz/Article/details/gwyrbfvmr.sHtML

[S19] C：快速排序
来源：http://blog.fanxiaobao.xyz/Article/details/gzketpsbf.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.fanxiaobao.xyz/Article/details/gompytklg.sHtML

[S20] C：二分查找
来源：http://baike.fanxiaobao.xyz/Article/details/gtwsoafbi.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.fanxiaobao.xyz/Article/details/gigrunmnd.sHtML

[S21] C：字符类别判断
来源：http://blog.fanxiaobao.xyz/Article/details/gfakpbfro.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.fanxiaobao.xyz/Article/details/glruojsyb.sHtML

[S22] C：字符串转数字
来源：http://3g.fanxiaobao.xyz/Article/details/goesgsmce.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.fanxiaobao.xyz/Article/details/gpupvpwsx.sHtML

[S23] C：随机数
来源：http://read.share.fanxiaobao.xyz/Article/details/gfnxkkepl.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.fanxiaobao.xyz/Article/details/ghznabjxg.sHtML

[S24] C：获取本地时间
来源：http://wap.fanxiaobao.xyz/Article/details/gagoqxvbj.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.fanxiaobao.xyz/Article/details/gjuurufay.sHtML

[S25] C：内存拷贝
来源：http://3g.fanxiaobao.xyz/Article/details/gsbawphpq.sHtML

memcpy(dst, src, n);
来源：http://baike.fanxiaobao.xyz/Article/details/gtrsxhnen.sHtML

[S26] C：内存清零
来源：http://3g.fanxiaobao.xyz/Article/details/gfvdrrxwo.sHtML

memset(a, 0, sizeof a);
来源：http://3g.fanxiaobao.xyz/Article/details/garwedril.sHtML

[S27] C：定义常量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtsqswswt.sHtML

const double PI = 3.14159;
来源：http://baike.fanxiaobao.xyz/Article/details/gdwhgrcty.sHtML

[S28] C：静态变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gvnbkdfxb.sHtML

static int counter = 0;
来源：http://read.share.fanxiaobao.xyz/Article/details/gewyaagdw.sHtML

[S29] C：变参函数
来源：http://blog.fanxiaobao.xyz/Article/details/gsvwqsuqs.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.fanxiaobao.xyz/Article/details/gbcuyplad.sHtML

[S30] C：头文件保护
来源：http://m.share.fanxiaobao.xyz/Article/details/gcmdmybxr.sHtML

#ifndef X_H
来源：http://m.share.fanxiaobao.xyz/Article/details/gjpxbmvzk.sHtML

#define X_H
来源：http://www.share.fanxiaobao.xyz/Article/details/girggwdju.sHtML

#endif
来源：http://3g.fanxiaobao.xyz/Article/details/gcuzysoru.sHtML

[S31] C++：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gagaroqob.sHtML

#include <iostream>
来源：http://mobile.fanxiaobao.xyz/Article/details/gjczhynho.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gzqhgewpd.sHtML

[S32] C++：字符串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gukobzvbj.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.fanxiaobao.xyz/Article/details/gbktnmdew.sHtML

[S33] C++：vector 增删
来源：http://m.share.fanxiaobao.xyz/Article/details/gfuqvgmfg.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.fanxiaobao.xyz/Article/details/glqtslgut.sHtML

[S34] C++：遍历 vector
来源：http://3g.fanxiaobao.xyz/Article/details/gjykpglne.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gvisxvaau.sHtML

[S35] C++：map
来源：http://3g.fanxiaobao.xyz/Article/details/gfxluwwpm.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gekxaumle.sHtML

[S36] C++：unordered_map
来源：http://wap.fanxiaobao.xyz/Article/details/gczxayaxg.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gcazdttyn.sHtML

[S37] C++：set
来源：http://www.share.fanxiaobao.xyz/Article/details/gtqpbfzoq.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.fanxiaobao.xyz/Article/details/gstpuijia.sHtML

[S38] C++：排序
来源：http://wap.fanxiaobao.xyz/Article/details/gckcfppry.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.fanxiaobao.xyz/Article/details/guhceluxd.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.fanxiaobao.xyz/Article/details/gsbwtgded.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gutfgphqs.sHtML

[S40] C++：查找元素
来源：http://www.share.fanxiaobao.xyz/Article/details/gieecmsqa.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grivwkkgi.sHtML

[S41] C++：类与构造函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gluxudvgz.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.fanxiaobao.xyz/Article/details/gxsciyogn.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gpjjwbukr.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.fanxiaobao.xyz/Article/details/gwwoyetqv.sHtML

[S43] C++：智能指针
来源：http://mobile.fanxiaobao.xyz/Article/details/gqarskeye.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.fanxiaobao.xyz/Article/details/gsvizeppx.sHtML

[S44] C++：引用传参
来源：http://www.share.fanxiaobao.xyz/Article/details/gpnmizzvf.sHtML

void inc(int &x) { ++x; }
来源：http://blog.fanxiaobao.xyz/Article/details/gbsyidsna.sHtML

[S45] C++：lambda
来源：http://3g.fanxiaobao.xyz/Article/details/gtzzzmvju.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.fanxiaobao.xyz/Article/details/ggfvdzslz.sHtML

[S46] C++：函数模板
来源：http://www.share.fanxiaobao.xyz/Article/details/gnpquxfsf.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.fanxiaobao.xyz/Article/details/gihirdevd.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.fanxiaobao.xyz/Article/details/gcftshiva.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsemhsagw.sHtML

[S48] C++：逐行读文件
来源：http://mobile.fanxiaobao.xyz/Article/details/guioukscp.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.fanxiaobao.xyz/Article/details/giyajcvut.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfcimbtpv.sHtML

[S49] C++：写文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gkidpjodi.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.fanxiaobao.xyz/Article/details/gmydztfqr.sHtML

[S50] C++：格式化数字
来源：http://m.share.fanxiaobao.xyz/Article/details/glzsbtgvn.sHtML


<!-- 参考信息 -->