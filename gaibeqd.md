代发 wailian999

[Q80] 字符串截取
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giwggqzin.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gvztjmpnn.sHtML

[Q81] 字符串替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnxggjzyp.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gnrepfvtn.sHtML

[Q82] 字符长度与字节长度
来源：http://blog.fanxiaobao.xyz/Article/details/gcbbdxprl.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/ggesnwfyv.sHtML

[Q83] 大小写转换
来源：http://wap.fanxiaobao.xyz/Article/details/gwqlqdzwa.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/ggobfvywc.sHtML

[Q84] 去除首尾空格
来源：http://mobile.fanxiaobao.xyz/Article/details/grmpbxtfm.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gghhicstd.sHtML

[Q85] 数值取整
来源：http://wap.fanxiaobao.xyz/Article/details/glkxlwdge.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://read.share.fanxiaobao.xyz/Article/details/gfmecpnlg.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.fanxiaobao.xyz/Article/details/gmmoadryo.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.fanxiaobao.xyz/Article/details/gdtkftnlt.sHtML

[Q87] JSON 字段做条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkyucbpyw.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.fanxiaobao.xyz/Article/details/gejdatycz.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.fanxiaobao.xyz/Article/details/gsqlrrzbg.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://blog.fanxiaobao.xyz/Article/details/gwhnaprup.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gcxcnpakf.sHtML

[Q89] 判断表是否存在
来源：http://www.share.fanxiaobao.xyz/Article/details/gueqkhpim.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wap.fanxiaobao.xyz/Article/details/ghwgxmgnu.sHtML

[Q90] 生成序号列
来源：http://www.share.fanxiaobao.xyz/Article/details/gridnxxec.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.fanxiaobao.xyz/Article/details/gqchhzrrg.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gqpovkgmz.sHtML

R. Bash 专题
来源：http://www.share.fanxiaobao.xyz/Article/details/gqfejolan.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gtynmgjlc.sHtML

[R01] shebang 与严格模式
来源：http://3g.fanxiaobao.xyz/Article/details/ghxzsceji.sHtML

#!/usr/bin/env bash
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggqzhukij.sHtML

set -euo pipefail
来源：http://mobile.fanxiaobao.xyz/Article/details/gyjcnyxhl.sHtML

[R02] 变量赋值与使用
来源：http://read.share.fanxiaobao.xyz/Article/details/glaqvhnvh.sHtML

name="Tom"; echo "$name"
来源：http://wap.fanxiaobao.xyz/Article/details/govemljdi.sHtML

[R03] 只读变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gewxfaztj.sHtML

readonly PI=3.14
来源：http://www.share.fanxiaobao.xyz/Article/details/gdpzsjzbj.sHtML

[R04] 位置参数
来源：http://www.share.fanxiaobao.xyz/Article/details/gevbsbqrw.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxchxurma.sHtML

[R05] 参数默认值
来源：http://read.share.fanxiaobao.xyz/Article/details/gheybuwcw.sHtML

name="${1:-default}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gwbqlttdw.sHtML

[R06] 判断命令是否存在
来源：http://baike.fanxiaobao.xyz/Article/details/gbvjbztxk.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/genwslqcf.sHtML

[R07] if 判断文件
来源：http://www.share.fanxiaobao.xyz/Article/details/geuuwxncg.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.fanxiaobao.xyz/Article/details/gywclhzes.sHtML

[R08] 数值比较
来源：http://3g.fanxiaobao.xyz/Article/details/gwyyccgbn.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/gioxgntyd.sHtML

[R09] 字符串比较
来源：http://mobile.fanxiaobao.xyz/Article/details/grecnzmyo.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.fanxiaobao.xyz/Article/details/gylvkapza.sHtML

[R10] 正则匹配
来源：http://read.share.fanxiaobao.xyz/Article/details/gqsvkcmty.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.fanxiaobao.xyz/Article/details/gdvvbgbdm.sHtML

[R11] case 多分支
来源：http://mobile.fanxiaobao.xyz/Article/details/gpgygqfud.sHtML

case "$1" in
来源：http://3g.fanxiaobao.xyz/Article/details/gbnvgccux.sHtML

start) echo "启动" ;;
来源：http://mobile.fanxiaobao.xyz/Article/details/gcweiugzh.sHtML

stop)  echo "停止" ;;
来源：http://read.share.fanxiaobao.xyz/Article/details/ghyqqghug.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.fanxiaobao.xyz/Article/details/ghpbuycjl.sHtML

esac
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfxbcgjuu.sHtML

[R12] for 遍历文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/grgnxluaf.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gueygkosr.sHtML

[R13] for 计数循环
来源：http://www.blog.fanxiaobao.xyz/Article/details/geislheqy.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggrealbdu.sHtML

[R14] C 风格 for
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmlvsatpw.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gixoukuzd.sHtML

[R15] while 逐行读文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gqifssekj.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gnrjlnwwv.sHtML

[R16] until 等待条件
来源：http://wap.fanxiaobao.xyz/Article/details/ghkmocwvh.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnpfzemfp.sHtML

[R17] 数组定义与取值
来源：http://m.share.fanxiaobao.xyz/Article/details/gagnxsdth.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://wap.fanxiaobao.xyz/Article/details/gdskduehq.sHtML

[R18] 遍历数组
来源：http://baike.fanxiaobao.xyz/Article/details/gsdvmxxhb.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gstllrmhz.sHtML

[R19] 数组长度
来源：http://www.share.fanxiaobao.xyz/Article/details/gxbytrwpr.sHtML

echo "${#arr[@]}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gabuyuyxx.sHtML

[R20] 关联数组（字典）
来源：http://m.share.fanxiaobao.xyz/Article/details/gonnxpbgh.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gcuusvrwj.sHtML

[R21] 字符串长度
来源：http://blog.fanxiaobao.xyz/Article/details/gntcfrlxr.sHtML

echo "${#s}"
来源：http://3g.fanxiaobao.xyz/Article/details/gefbuhanf.sHtML

[R22] 截取子串
来源：http://mobile.fanxiaobao.xyz/Article/details/gqxldatmz.sHtML

echo "${s:0:5}"
来源：http://3g.fanxiaobao.xyz/Article/details/gvrvexrpo.sHtML

[R23] 字符串替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gndidjgtj.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.fanxiaobao.xyz/Article/details/gusaifmwm.sHtML

[R24] 大小写转换
来源：http://read.share.fanxiaobao.xyz/Article/details/gmchznvto.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gdkyitkor.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.fanxiaobao.xyz/Article/details/gbugzntth.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.fanxiaobao.xyz/Article/details/gqrrrxpyq.sHtML

[R26] 命令替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gaurtbyoh.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.fanxiaobao.xyz/Article/details/gtkldwizw.sHtML

[R27] 算术展开
来源：http://3g.fanxiaobao.xyz/Article/details/gyiwsdiom.sHtML

echo $((1 + 2 * 3))
来源：http://baike.fanxiaobao.xyz/Article/details/gofsoovcz.sHtML

[R28] 浮点运算
来源：http://m.share.fanxiaobao.xyz/Article/details/goivlmllr.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyyzcrkxe.sHtML

[R29] 定义函数
来源：http://baike.fanxiaobao.xyz/Article/details/gnjpdcmyf.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.fanxiaobao.xyz/Article/details/gtxaydcoj.sHtML

[R30] 函数返回状态码
来源：http://wap.fanxiaobao.xyz/Article/details/gzyquvdtv.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.fanxiaobao.xyz/Article/details/gprdyioqk.sHtML

[R31] 局部变量
来源：http://blog.fanxiaobao.xyz/Article/details/goxmglzkw.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxsorpbll.sHtML

[R32] 参数个数校验
来源：http://blog.fanxiaobao.xyz/Article/details/gvwfwjkjo.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpptwsunp.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.fanxiaobao.xyz/Article/details/gqjpnyrzb.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.fanxiaobao.xyz/Article/details/gzedtpcet.sHtML

[R34] 退出时清理
来源：http://baike.fanxiaobao.xyz/Article/details/ghrnbqsca.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fanxiaobao.xyz/Article/details/gpurlaxrj.sHtML

[R35] 后台执行并等待
来源：http://read.share.fanxiaobao.xyz/Article/details/gxxgtjyyp.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.fanxiaobao.xyz/Article/details/grouyrxzc.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtcfszzeo.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.fanxiaobao.xyz/Article/details/gsnplyiri.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvvggaaba.sHtML

files=$(ls -1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gejhbfamd.sHtML

[R38] 管道串联
来源：http://blog.fanxiaobao.xyz/Article/details/gtdpmasmb.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.fanxiaobao.xyz/Article/details/gnsztgknr.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.fanxiaobao.xyz/Article/details/gnuyxmdgj.sHtML

cmd > out.log 2>&1
来源：http://read.share.fanxiaobao.xyz/Article/details/gzkyeqdox.sHtML

[R40] 追加写日志
来源：http://mobile.fanxiaobao.xyz/Article/details/gqeeaxrmq.sHtML

echo "log" >> out.log
来源：http://mobile.fanxiaobao.xyz/Article/details/ggniofuqd.sHtML

[R41] 丢弃输出
来源：http://baike.fanxiaobao.xyz/Article/details/gqrmrhcjh.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvogabcql.sHtML

[R42] 输入重定向
来源：http://baike.fanxiaobao.xyz/Article/details/gtdzgmkht.sHtML

wc -l < a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gyewwojdm.sHtML

[R43] 按名字查找文件
来源：http://wap.fanxiaobao.xyz/Article/details/gxkgtumeg.sHtML

find . -name "*.log" -type f
来源：http://read.share.fanxiaobao.xyz/Article/details/gkrlobfrf.sHtML

[R44] 按修改时间查找
来源：http://mobile.fanxiaobao.xyz/Article/details/gcgzhpplh.sHtML

find . -mtime -7 -type f
来源：http://read.share.fanxiaobao.xyz/Article/details/gmhjdptkx.sHtML

[R45] 批量删除
来源：http://wap.fanxiaobao.xyz/Article/details/gydyriamv.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.fanxiaobao.xyz/Article/details/gazpmhewv.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpxrhfcie.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://m.share.fanxiaobao.xyz/Article/details/gxssvrqid.sHtML

[R47] sed 单行替换
来源：http://3g.fanxiaobao.xyz/Article/details/gxsypaxsy.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/ggfmlhxqk.sHtML

[R48] awk 取指定列
来源：http://mobile.fanxiaobao.xyz/Article/details/gtgatqgho.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gkyrgipkv.sHtML

[R49] awk 带条件
来源：http://read.share.fanxiaobao.xyz/Article/details/gswgnfxmh.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfvqyvnnk.sHtML

[R50] awk 求和
来源：http://mobile.fanxiaobao.xyz/Article/details/gkasdzafk.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/ghwayrjfi.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geuzmaojt.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.fanxiaobao.xyz/Article/details/gwslyfoba.sHtML

[R52] 统计行数
来源：http://wap.fanxiaobao.xyz/Article/details/gmoecjcog.sHtML

wc -l a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdrxhokos.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.fanxiaobao.xyz/Article/details/gnqvmssgu.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.fanxiaobao.xyz/Article/details/gctkipoyb.sHtML

[R54] 比较两个文件
来源：http://mobile.fanxiaobao.xyz/Article/details/ghpxaanml.sHtML

diff a.txt b.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gheyrvixo.sHtML

[R55] 压缩与解压
来源：http://mobile.fanxiaobao.xyz/Article/details/ghyoqizvj.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.fanxiaobao.xyz/Article/details/gwwkuromf.sHtML

[R56] 远程拷贝
来源：http://m.share.fanxiaobao.xyz/Article/details/gqkxqmrsc.sHtML

scp file user@host:/path/
来源：http://www.share.fanxiaobao.xyz/Article/details/ghvjltved.sHtML

[R57] 远程执行命令
来源：http://wap.fanxiaobao.xyz/Article/details/gyqzrttsx.sHtML

ssh user@host 'uptime'
来源：http://3g.fanxiaobao.xyz/Article/details/gylbrwdki.sHtML

[R58] 下载文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gayoodmcs.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.fanxiaobao.xyz/Article/details/gumyvzzia.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzbpnkwnk.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggevcumen.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.fanxiaobao.xyz/Article/details/gqzrxcjan.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.fanxiaobao.xyz/Article/details/gfinefxjl.sHtML

[R61] 磁盘占用
来源：http://wap.fanxiaobao.xyz/Article/details/gdybxioxn.sHtML

df -h;  du -sh *
来源：http://mobile.fanxiaobao.xyz/Article/details/gsdxobdfl.sHtML

[R62] 找最占空间的文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gcoadgqll.sHtML

du -ah . | sort -rh | head -10
来源：http://3g.fanxiaobao.xyz/Article/details/gswodzqih.sHtML

[R63] 内存与进程
来源：http://baike.fanxiaobao.xyz/Article/details/gmrbyeifc.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.fanxiaobao.xyz/Article/details/grzwjvrrs.sHtML

[R64] 结束进程
来源：http://baike.fanxiaobao.xyz/Article/details/gijbbwvxd.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.fanxiaobao.xyz/Article/details/gtaptdcqp.sHtML

[R65] 查看端口占用
来源：http://baike.fanxiaobao.xyz/Article/details/ggfbznasw.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.fanxiaobao.xyz/Article/details/gjdxjqobt.sHtML

[R66] 定时任务
来源：http://blog.fanxiaobao.xyz/Article/details/gvrcgkirs.sHtML

crontab -e;  crontab -l
来源：http://read.share.fanxiaobao.xyz/Article/details/gwdunizcp.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.fanxiaobao.xyz/Article/details/gfjxwpoiq.sHtML

openssl rand -hex 16
来源：http://wap.fanxiaobao.xyz/Article/details/geoxshwzf.sHtML

[R68] 计算文件校验值
来源：http://blog.fanxiaobao.xyz/Article/details/gegiuyopc.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gslugpush.sHtML

[R69] 生成随机密码
来源：http://3g.fanxiaobao.xyz/Article/details/gdmrbgypc.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.fanxiaobao.xyz/Article/details/gsvzehdjv.sHtML

[R70] 时间戳与互转
来源：http://3g.fanxiaobao.xyz/Article/details/gsbmczexs.sHtML

date +%s;  date -d @1700000000
来源：http://wap.fanxiaobao.xyz/Article/details/gyazxbgly.sHtML

[R71] 日期格式化
来源：http://blog.fanxiaobao.xyz/Article/details/gcdorkzmo.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.fanxiaobao.xyz/Article/details/gwqanunpz.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjlxujzxh.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gpqvsrnfq.sHtML

[R73] 分割大日志
来源：http://blog.fanxiaobao.xyz/Article/details/gqroexczm.sHtML

split -l 1000 big.log part_
来源：http://m.share.fanxiaobao.xyz/Article/details/gmifixoyz.sHtML

[R74] 批量重命名
来源：http://blog.fanxiaobao.xyz/Article/details/gxpvorowf.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.fanxiaobao.xyz/Article/details/gnkguqooq.sHtML

[R75] 导出环境变量
来源：http://baike.fanxiaobao.xyz/Article/details/grhvvtotl.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaopumcrr.sHtML

[R76] 使用临时文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gulbffdgn.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.fanxiaobao.xyz/Article/details/gvnvktczl.sHtML

[R77] 读取用户输入
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqmwxdnnc.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbjyoujgp.sHtML

[R78] 交互式菜单
来源：http://mobile.fanxiaobao.xyz/Article/details/gnenktrrf.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.fanxiaobao.xyz/Article/details/gtlokpdxh.sHtML

[R79] 解析命令行选项
来源：http://mobile.fanxiaobao.xyz/Article/details/gzptnifnj.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gacsmyqoq.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.fanxiaobao.xyz/Article/details/gvcngurkn.sHtML

time ./run.sh
来源：http://m.share.fanxiaobao.xyz/Article/details/grlvfhbez.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gmzeharxe.sHtML

S. C / C++ 专题
来源：http://baike.fanxiaobao.xyz/Article/details/gkjiziban.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyvtvhrcq.sHtML

[S01] C：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/ghxuedvue.sHtML

#include <stdio.h>
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnxmocuvo.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.fanxiaobao.xyz/Article/details/gqpssbuqa.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.fanxiaobao.xyz/Article/details/grwvyyamq.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.fanxiaobao.xyz/Article/details/gxcnxwzkz.sHtML

[S03] C：读入整数
来源：http://3g.fanxiaobao.xyz/Article/details/gxjqzhbsf.sHtML

int x; scanf("%d", &x);
来源：http://3g.fanxiaobao.xyz/Article/details/galwbzmux.sHtML

[S04] C：字符串复制
来源：http://www.blog.fanxiaobao.xyz/Article/details/gamkxbdod.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.fanxiaobao.xyz/Article/details/giivvyvzz.sHtML

[S05] C：字符串长度
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfbyrxyfl.sHtML

strlen(s)
来源：http://mobile.fanxiaobao.xyz/Article/details/gtcasfbfb.sHtML

[S06] C：字符串比较
来源：http://m.share.fanxiaobao.xyz/Article/details/gfsjbprpa.sHtML

strcmp(a, b) == 0
来源：http://m.share.fanxiaobao.xyz/Article/details/gaotignrb.sHtML

[S07] C：数组遍历求和
来源：http://mobile.fanxiaobao.xyz/Article/details/gocmwyece.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.fanxiaobao.xyz/Article/details/gxapjrfir.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.fanxiaobao.xyz/Article/details/gmgeeoxwy.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.fanxiaobao.xyz/Article/details/gvvptbuqz.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guhlgahpk.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.fanxiaobao.xyz/Article/details/gzzupszgl.sHtML

[S10] C：指针与解引用
来源：http://wap.fanxiaobao.xyz/Article/details/gfplvycel.sHtML

int *p = &a;  *p = 5;
来源：http://wap.fanxiaobao.xyz/Article/details/goajpsdfm.sHtML

[S11] C：逐行读文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gtjxykmid.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.fanxiaobao.xyz/Article/details/gtcojzsyb.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gieouhbpc.sHtML

fclose(f);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcxantbbu.sHtML

[S12] C：写文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gvetbvvnd.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.fanxiaobao.xyz/Article/details/gmqtvtmcp.sHtML

[S13] C：宏定义
来源：http://blog.fanxiaobao.xyz/Article/details/gjoeufnut.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmuhaiuyh.sHtML

[S14] C：枚举
来源：http://blog.fanxiaobao.xyz/Article/details/gptdgjkpr.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.fanxiaobao.xyz/Article/details/gdnqxjgob.sHtML

[S15] C：类型转换
来源：http://read.share.fanxiaobao.xyz/Article/details/gjcvhmcnv.sHtML

(double) a / b
来源：http://mobile.fanxiaobao.xyz/Article/details/gbxhblecb.sHtML

[S16] C：位操作置位
来源：http://mobile.fanxiaobao.xyz/Article/details/gmstlykuq.sHtML

x |= (1 << 3);
来源：http://read.share.fanxiaobao.xyz/Article/details/gfvjnwwsc.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gowuxwoxm.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.fanxiaobao.xyz/Article/details/gorhqkpep.sHtML

[S18] C：命令行参数
来源：http://mobile.fanxiaobao.xyz/Article/details/gvnhmwexv.sHtML

int main(int argc, char **argv)
来源：http://www.share.fanxiaobao.xyz/Article/details/gesrlbplp.sHtML

[S19] C：快速排序
来源：http://3g.fanxiaobao.xyz/Article/details/gbuhpwbmv.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.fanxiaobao.xyz/Article/details/gzbbamaec.sHtML

[S20] C：二分查找
来源：http://m.share.fanxiaobao.xyz/Article/details/gdbirggtg.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.fanxiaobao.xyz/Article/details/gyvwpncyb.sHtML

[S21] C：字符类别判断
来源：http://baike.fanxiaobao.xyz/Article/details/gikglknxw.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.fanxiaobao.xyz/Article/details/gnwbdgjuc.sHtML

[S22] C：字符串转数字
来源：http://3g.fanxiaobao.xyz/Article/details/gipbxdbng.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.fanxiaobao.xyz/Article/details/ghkmuihsx.sHtML

[S23] C：随机数
来源：http://blog.fanxiaobao.xyz/Article/details/gwzawysuu.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.fanxiaobao.xyz/Article/details/gmskwnwdz.sHtML

[S24] C：获取本地时间
来源：http://mobile.fanxiaobao.xyz/Article/details/gqtvweycs.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.fanxiaobao.xyz/Article/details/gqsbgfzow.sHtML

[S25] C：内存拷贝
来源：http://m.share.fanxiaobao.xyz/Article/details/giyezfjqx.sHtML

memcpy(dst, src, n);
来源：http://wap.fanxiaobao.xyz/Article/details/giejfghct.sHtML

[S26] C：内存清零
来源：http://mobile.fanxiaobao.xyz/Article/details/ggswcbmit.sHtML

memset(a, 0, sizeof a);
来源：http://blog.fanxiaobao.xyz/Article/details/gsvweaqnn.sHtML

[S27] C：定义常量
来源：http://baike.fanxiaobao.xyz/Article/details/gplxkpths.sHtML

const double PI = 3.14159;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqfmtmzyt.sHtML

[S28] C：静态变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbhfshyto.sHtML

static int counter = 0;
来源：http://read.share.fanxiaobao.xyz/Article/details/gxkwrzrfd.sHtML

[S29] C：变参函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gunzqvrgz.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.fanxiaobao.xyz/Article/details/ggfrghdyd.sHtML

[S30] C：头文件保护
来源：http://3g.fanxiaobao.xyz/Article/details/gdelmuqhi.sHtML

#ifndef X_H
来源：http://baike.fanxiaobao.xyz/Article/details/gsqeecjuc.sHtML

#define X_H
来源：http://3g.fanxiaobao.xyz/Article/details/glzcqhzyj.sHtML

#endif
来源：http://www.share.fanxiaobao.xyz/Article/details/grrtbjhzk.sHtML

[S31] C++：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/geavpgpji.sHtML

#include <iostream>
来源：http://m.share.fanxiaobao.xyz/Article/details/gbwvmewhs.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/ggaotspvc.sHtML

[S32] C++：字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/gqwukwrzn.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.fanxiaobao.xyz/Article/details/gkfohomue.sHtML

[S33] C++：vector 增删
来源：http://www.blog.fanxiaobao.xyz/Article/details/giguqexuh.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.fanxiaobao.xyz/Article/details/gekfdekms.sHtML

[S34] C++：遍历 vector
来源：http://read.share.fanxiaobao.xyz/Article/details/geettdjvq.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.fanxiaobao.xyz/Article/details/gmkndjfvp.sHtML

[S35] C++：map
来源：http://mobile.fanxiaobao.xyz/Article/details/gyjtmnhod.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.fanxiaobao.xyz/Article/details/gyxgzycll.sHtML

[S36] C++：unordered_map
来源：http://mobile.fanxiaobao.xyz/Article/details/gzdlyixhf.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gchsewfzl.sHtML

[S37] C++：set
来源：http://blog.fanxiaobao.xyz/Article/details/glzvycoee.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.fanxiaobao.xyz/Article/details/gkgjzronm.sHtML

[S38] C++：排序
来源：http://blog.fanxiaobao.xyz/Article/details/gjpeefpiz.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.fanxiaobao.xyz/Article/details/gktosiffa.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.fanxiaobao.xyz/Article/details/geappriru.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.fanxiaobao.xyz/Article/details/gsdvjckez.sHtML

[S40] C++：查找元素
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvvlodcyl.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.fanxiaobao.xyz/Article/details/gdvfmifjw.sHtML

[S41] C++：类与构造函数
来源：http://3g.fanxiaobao.xyz/Article/details/gyfchnkql.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.fanxiaobao.xyz/Article/details/gtvzntzmw.sHtML

[S42] C++：继承与虚函数
来源：http://3g.fanxiaobao.xyz/Article/details/gwfjziqac.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.fanxiaobao.xyz/Article/details/gvwwriopn.sHtML

[S43] C++：智能指针
来源：http://3g.fanxiaobao.xyz/Article/details/gvubsirtx.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfrkswctn.sHtML

[S44] C++：引用传参
来源：http://3g.fanxiaobao.xyz/Article/details/gpdzusgon.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqvtojaxz.sHtML

[S45] C++：lambda
来源：http://blog.fanxiaobao.xyz/Article/details/gzepczqlq.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwzbytyej.sHtML

[S46] C++：函数模板
来源：http://blog.fanxiaobao.xyz/Article/details/gwetstoou.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.fanxiaobao.xyz/Article/details/gsunndtnf.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.fanxiaobao.xyz/Article/details/ggobbyscr.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcocgnzjf.sHtML

[S48] C++：逐行读文件
来源：http://3g.fanxiaobao.xyz/Article/details/gwaelfonh.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggdygoqkv.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.fanxiaobao.xyz/Article/details/gezfyboza.sHtML

[S49] C++：写文件
来源：http://wap.fanxiaobao.xyz/Article/details/gzqqvoamj.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.fanxiaobao.xyz/Article/details/gmlwkjdlm.sHtML

[S50] C++：格式化数字
来源：http://m.share.fanxiaobao.xyz/Article/details/ggvhplyzk.sHtML


<!-- 参考信息 -->