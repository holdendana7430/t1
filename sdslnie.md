代发 wailian999

[Q88] 行转列（条件聚合）
来源：http://www.share.fanxiaobao.xyz/Article/details/gowoezizd.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://baike.fanxiaobao.xyz/Article/details/gvoyjwczd.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjlmywmzx.sHtML

[Q89] 判断表是否存在
来源：http://mobile.fanxiaobao.xyz/Article/details/gdmefhjth.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gztjlufia.sHtML

[Q90] 生成序号列
来源：http://mobile.fanxiaobao.xyz/Article/details/gpponcmoa.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://read.share.fanxiaobao.xyz/Article/details/gfyqyfccp.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/guwydljux.sHtML

R. Bash 专题
来源：http://read.share.fanxiaobao.xyz/Article/details/gwvzivxjr.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/ggadjwcan.sHtML

[R01] shebang 与严格模式
来源：http://wap.fanxiaobao.xyz/Article/details/glcbimiaw.sHtML

#!/usr/bin/env bash
来源：http://mobile.fanxiaobao.xyz/Article/details/gbsfezutz.sHtML

set -euo pipefail
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggdqrhelg.sHtML

[R02] 变量赋值与使用
来源：http://baike.fanxiaobao.xyz/Article/details/gnvphkaxx.sHtML

name="Tom"; echo "$name"
来源：http://www.share.fanxiaobao.xyz/Article/details/gtgbmzaqc.sHtML

[R03] 只读变量
来源：http://3g.fanxiaobao.xyz/Article/details/gqfsjisye.sHtML

readonly PI=3.14
来源：http://wap.fanxiaobao.xyz/Article/details/gykcunsil.sHtML

[R04] 位置参数
来源：http://wap.fanxiaobao.xyz/Article/details/ghetrobyl.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.fanxiaobao.xyz/Article/details/gmezzbbda.sHtML

[R05] 参数默认值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gflppndsx.sHtML

name="${1:-default}"
来源：http://3g.fanxiaobao.xyz/Article/details/gldjniuoi.sHtML

[R06] 判断命令是否存在
来源：http://wap.fanxiaobao.xyz/Article/details/glpbqexml.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glszuflxd.sHtML

[R07] if 判断文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gggtcvzua.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://baike.fanxiaobao.xyz/Article/details/gzegyvrii.sHtML

[R08] 数值比较
来源：http://3g.fanxiaobao.xyz/Article/details/gvvynvnoi.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://m.share.fanxiaobao.xyz/Article/details/gcxqykqui.sHtML

[R09] 字符串比较
来源：http://www.m.share.fanxiaobao.xyz/Article/details/getpzaqls.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.fanxiaobao.xyz/Article/details/gftktekjv.sHtML

[R10] 正则匹配
来源：http://baike.fanxiaobao.xyz/Article/details/gauiqpzmd.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtdengwon.sHtML

[R11] case 多分支
来源：http://blog.fanxiaobao.xyz/Article/details/gsickyhrw.sHtML

case "$1" in
来源：http://baike.fanxiaobao.xyz/Article/details/gcotnyehj.sHtML

start) echo "启动" ;;
来源：http://m.share.fanxiaobao.xyz/Article/details/geakdeljl.sHtML

stop)  echo "停止" ;;
来源：http://blog.fanxiaobao.xyz/Article/details/gxlsewdlb.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.fanxiaobao.xyz/Article/details/gwiggxguc.sHtML

esac
来源：http://www.share.fanxiaobao.xyz/Article/details/grvvuvmgr.sHtML

[R12] for 遍历文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gxavaofag.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.fanxiaobao.xyz/Article/details/gutpmeznv.sHtML

[R13] for 计数循环
来源：http://blog.fanxiaobao.xyz/Article/details/gyayhpewy.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gcmjkqcgj.sHtML

[R14] C 风格 for
来源：http://wap.fanxiaobao.xyz/Article/details/gbbcdznzh.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnrcunosb.sHtML

[R15] while 逐行读文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gjajihctx.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gofpkuhir.sHtML

[R16] until 等待条件
来源：http://wap.fanxiaobao.xyz/Article/details/gqceglujf.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.fanxiaobao.xyz/Article/details/gzgdsefyj.sHtML

[R17] 数组定义与取值
来源：http://wap.fanxiaobao.xyz/Article/details/gjglfucvl.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/guuoosrst.sHtML

[R18] 遍历数组
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqdtycqbk.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gxcqzyxlr.sHtML

[R19] 数组长度
来源：http://m.share.fanxiaobao.xyz/Article/details/gkvtomupf.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpkhfovgm.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glubthghh.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxgtpjxof.sHtML

[R21] 字符串长度
来源：http://blog.fanxiaobao.xyz/Article/details/gtmdoixgj.sHtML

echo "${#s}"
来源：http://3g.fanxiaobao.xyz/Article/details/gmcykylgz.sHtML

[R22] 截取子串
来源：http://3g.fanxiaobao.xyz/Article/details/gwvoeibio.sHtML

echo "${s:0:5}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gteuojfar.sHtML

[R23] 字符串替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gtdmgehpz.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.fanxiaobao.xyz/Article/details/grxpsfpvf.sHtML

[R24] 大小写转换
来源：http://m.share.fanxiaobao.xyz/Article/details/gcmtovyxx.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.fanxiaobao.xyz/Article/details/gstlwhrfx.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.fanxiaobao.xyz/Article/details/gndbgebtx.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvanwdkta.sHtML

[R26] 命令替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gqdhfftdf.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.fanxiaobao.xyz/Article/details/gxaqjlgrd.sHtML

[R27] 算术展开
来源：http://3g.fanxiaobao.xyz/Article/details/gynbocelt.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gptwqpetf.sHtML

[R28] 浮点运算
来源：http://www.share.fanxiaobao.xyz/Article/details/gfenykbpq.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.fanxiaobao.xyz/Article/details/gujhdcaal.sHtML

[R29] 定义函数
来源：http://3g.fanxiaobao.xyz/Article/details/ghoetyhpu.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.fanxiaobao.xyz/Article/details/gcunbaikl.sHtML

[R30] 函数返回状态码
来源：http://mobile.fanxiaobao.xyz/Article/details/guhguybfm.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.fanxiaobao.xyz/Article/details/gawtiarcv.sHtML

[R31] 局部变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gsnfyundg.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/grfsvctnp.sHtML

[R32] 参数个数校验
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkkgxwfsv.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gasmlskye.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.fanxiaobao.xyz/Article/details/gtebtwrvl.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkjajogxo.sHtML

[R34] 退出时清理
来源：http://mobile.fanxiaobao.xyz/Article/details/gxjhadbqi.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.fanxiaobao.xyz/Article/details/gdnkcfslt.sHtML

[R35] 后台执行并等待
来源：http://m.share.fanxiaobao.xyz/Article/details/gxddfycly.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.fanxiaobao.xyz/Article/details/gkllkvora.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.fanxiaobao.xyz/Article/details/guyeidymz.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.fanxiaobao.xyz/Article/details/gtlmsmfrb.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/guuiuezqc.sHtML

files=$(ls -1)
来源：http://3g.fanxiaobao.xyz/Article/details/gnneprgqr.sHtML

[R38] 管道串联
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glhphcivw.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcscklwkb.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gelpiajuc.sHtML

cmd > out.log 2>&1
来源：http://m.share.fanxiaobao.xyz/Article/details/gxrbiduaq.sHtML

[R40] 追加写日志
来源：http://wap.fanxiaobao.xyz/Article/details/gpuvjlygp.sHtML

echo "log" >> out.log
来源：http://3g.fanxiaobao.xyz/Article/details/gzjezjcpz.sHtML

[R41] 丢弃输出
来源：http://baike.fanxiaobao.xyz/Article/details/gdirhggsa.sHtML

cmd >/dev/null 2>&1
来源：http://baike.fanxiaobao.xyz/Article/details/gcpgugonc.sHtML

[R42] 输入重定向
来源：http://mobile.fanxiaobao.xyz/Article/details/gpbkuxmvv.sHtML

wc -l < a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gxvqhnmvx.sHtML

[R43] 按名字查找文件
来源：http://wap.fanxiaobao.xyz/Article/details/gzxrntlep.sHtML

find . -name "*.log" -type f
来源：http://baike.fanxiaobao.xyz/Article/details/gozsibfds.sHtML

[R44] 按修改时间查找
来源：http://read.share.fanxiaobao.xyz/Article/details/gjpoaeeip.sHtML

find . -mtime -7 -type f
来源：http://3g.fanxiaobao.xyz/Article/details/gbwiylvhi.sHtML

[R45] 批量删除
来源：http://baike.fanxiaobao.xyz/Article/details/gutxdxvzo.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.fanxiaobao.xyz/Article/details/gpqxmgtoc.sHtML

[R46] 递归替换文件内容
来源：http://read.share.fanxiaobao.xyz/Article/details/gojdigxnv.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.fanxiaobao.xyz/Article/details/gtiybkcny.sHtML

[R47] sed 单行替换
来源：http://www.share.fanxiaobao.xyz/Article/details/gkouizxlv.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gjryzocne.sHtML

[R48] awk 取指定列
来源：http://baike.fanxiaobao.xyz/Article/details/ghnzsnope.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/grstwjjuz.sHtML

[R49] awk 带条件
来源：http://wap.fanxiaobao.xyz/Article/details/gwjrkgngu.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.fanxiaobao.xyz/Article/details/ghdnhwunr.sHtML

[R50] awk 求和
来源：http://baike.fanxiaobao.xyz/Article/details/gkdfmdwfr.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gtudbxemm.sHtML

[R51] 排序去重取前几
来源：http://mobile.fanxiaobao.xyz/Article/details/gpgiebfdc.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.fanxiaobao.xyz/Article/details/gbmdfkpdo.sHtML

[R52] 统计行数
来源：http://www.share.fanxiaobao.xyz/Article/details/gmqvhjzsi.sHtML

wc -l a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gqutlydrg.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.fanxiaobao.xyz/Article/details/gpgrgrmmd.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.fanxiaobao.xyz/Article/details/glfdkgulr.sHtML

[R54] 比较两个文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gymsdxlgr.sHtML

diff a.txt b.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gqbjupgte.sHtML

[R55] 压缩与解压
来源：http://wap.fanxiaobao.xyz/Article/details/grjboseuq.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.fanxiaobao.xyz/Article/details/gexmjxjth.sHtML

[R56] 远程拷贝
来源：http://baike.fanxiaobao.xyz/Article/details/gpmarxwcx.sHtML

scp file user@host:/path/
来源：http://blog.fanxiaobao.xyz/Article/details/ggxuwohuo.sHtML

[R57] 远程执行命令
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guhzijsdt.sHtML

ssh user@host 'uptime'
来源：http://wap.fanxiaobao.xyz/Article/details/ggdyjbvgu.sHtML

[R58] 下载文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gqucjeghy.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.fanxiaobao.xyz/Article/details/gdfxstayq.sHtML

[R59] 发 POST JSON
来源：http://www.share.fanxiaobao.xyz/Article/details/gwodfhdhv.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.fanxiaobao.xyz/Article/details/geeqvtscx.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmcokoquq.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.fanxiaobao.xyz/Article/details/gtwhjpqvk.sHtML

[R61] 磁盘占用
来源：http://read.share.fanxiaobao.xyz/Article/details/gbxagtezi.sHtML

df -h;  du -sh *
来源：http://m.share.fanxiaobao.xyz/Article/details/gweggwozk.sHtML

[R62] 找最占空间的文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gxehzimuw.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.fanxiaobao.xyz/Article/details/gzfyoraqk.sHtML

[R63] 内存与进程
来源：http://m.share.fanxiaobao.xyz/Article/details/gloaeirzu.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.fanxiaobao.xyz/Article/details/gxuvmngju.sHtML

[R64] 结束进程
来源：http://read.share.fanxiaobao.xyz/Article/details/gsaorzzbb.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.fanxiaobao.xyz/Article/details/gwwsmcikk.sHtML

[R65] 查看端口占用
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzmushldf.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsovsciqh.sHtML

[R66] 定时任务
来源：http://wap.fanxiaobao.xyz/Article/details/gvudnigpw.sHtML

crontab -e;  crontab -l
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfvlnetvv.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.fanxiaobao.xyz/Article/details/gyyebiexu.sHtML

openssl rand -hex 16
来源：http://www.blog.fanxiaobao.xyz/Article/details/giszbcqze.sHtML

[R68] 计算文件校验值
来源：http://blog.fanxiaobao.xyz/Article/details/gzykxkvxl.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gxawdaiyx.sHtML

[R69] 生成随机密码
来源：http://www.share.fanxiaobao.xyz/Article/details/gyhuqzfzt.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.fanxiaobao.xyz/Article/details/ghsgrbqjx.sHtML

[R70] 时间戳与互转
来源：http://read.share.fanxiaobao.xyz/Article/details/gxqnysmbx.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqkucmaaw.sHtML

[R71] 日期格式化
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyumlijnz.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzqynkwdm.sHtML

[R72] 等待端口就绪
来源：http://www.share.fanxiaobao.xyz/Article/details/gqesxeour.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.fanxiaobao.xyz/Article/details/gekfgwbmu.sHtML

[R73] 分割大日志
来源：http://baike.fanxiaobao.xyz/Article/details/gqfjqqpns.sHtML

split -l 1000 big.log part_
来源：http://m.share.fanxiaobao.xyz/Article/details/grwbxydxi.sHtML

[R74] 批量重命名
来源：http://baike.fanxiaobao.xyz/Article/details/gjyahiboi.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gvzzqzide.sHtML

[R75] 导出环境变量
来源：http://blog.fanxiaobao.xyz/Article/details/gplczivar.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.fanxiaobao.xyz/Article/details/gnjwwqirv.sHtML

[R76] 使用临时文件
来源：http://wap.fanxiaobao.xyz/Article/details/gexisnujs.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.fanxiaobao.xyz/Article/details/gkjbhbtds.sHtML

[R77] 读取用户输入
来源：http://wap.fanxiaobao.xyz/Article/details/gtpvfrpyz.sHtML

read -rp "请输入: " ans
来源：http://baike.fanxiaobao.xyz/Article/details/gbslngyen.sHtML

[R78] 交互式菜单
来源：http://baike.fanxiaobao.xyz/Article/details/gqbqpnifo.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkptwuifd.sHtML

[R79] 解析命令行选项
来源：http://3g.fanxiaobao.xyz/Article/details/gcvehbdwd.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.fanxiaobao.xyz/Article/details/giheruyvv.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.fanxiaobao.xyz/Article/details/gtpnhmqys.sHtML

time ./run.sh
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqayuvmpt.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gntythjju.sHtML

S. C / C++ 专题
来源：http://wap.fanxiaobao.xyz/Article/details/gienfthxs.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gqpibrszk.sHtML

[S01] C：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gomoqrmoz.sHtML

#include <stdio.h>
来源：http://3g.fanxiaobao.xyz/Article/details/grizbiclz.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.fanxiaobao.xyz/Article/details/ghxsxrdor.sHtML

[S02] C：变量与格式化输出
来源：http://wap.fanxiaobao.xyz/Article/details/gsagjppux.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.fanxiaobao.xyz/Article/details/glktpmgax.sHtML

[S03] C：读入整数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvxiqgqew.sHtML

int x; scanf("%d", &x);
来源：http://baike.fanxiaobao.xyz/Article/details/gvkhsfbkg.sHtML

[S04] C：字符串复制
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxgmjxbuj.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giwfkakde.sHtML

[S05] C：字符串长度
来源：http://blog.fanxiaobao.xyz/Article/details/grakfhgqz.sHtML

strlen(s)
来源：http://blog.fanxiaobao.xyz/Article/details/gotgxiqly.sHtML

[S06] C：字符串比较
来源：http://baike.fanxiaobao.xyz/Article/details/gufuqbqci.sHtML

strcmp(a, b) == 0
来源：http://wap.fanxiaobao.xyz/Article/details/gsqlgcdny.sHtML

[S07] C：数组遍历求和
来源：http://m.share.fanxiaobao.xyz/Article/details/gdanamevb.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.fanxiaobao.xyz/Article/details/gylpxearr.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.fanxiaobao.xyz/Article/details/gegoxsxns.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.fanxiaobao.xyz/Article/details/goesoygli.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.fanxiaobao.xyz/Article/details/grqoyclaf.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.fanxiaobao.xyz/Article/details/gkctspaon.sHtML

[S10] C：指针与解引用
来源：http://www.share.fanxiaobao.xyz/Article/details/gwrufzwfl.sHtML

int *p = &a;  *p = 5;
来源：http://baike.fanxiaobao.xyz/Article/details/gzuobjorj.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtbecapdp.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.fanxiaobao.xyz/Article/details/glvlivrjj.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.fanxiaobao.xyz/Article/details/gpqiwzkjt.sHtML

fclose(f);
来源：http://baike.fanxiaobao.xyz/Article/details/grrnxyumo.sHtML

[S12] C：写文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtnrmpwki.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.fanxiaobao.xyz/Article/details/gnpbugakl.sHtML

[S13] C：宏定义
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdxxafuch.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.fanxiaobao.xyz/Article/details/guhbxhofc.sHtML

[S14] C：枚举
来源：http://blog.fanxiaobao.xyz/Article/details/gaqzypkpd.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqatvxjyq.sHtML

[S15] C：类型转换
来源：http://www.share.fanxiaobao.xyz/Article/details/gbspstxwq.sHtML

(double) a / b
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkvyprylh.sHtML

[S16] C：位操作置位
来源：http://m.share.fanxiaobao.xyz/Article/details/gktrfrbsp.sHtML

x |= (1 << 3);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcnaqbwxe.sHtML

[S17] C：安全拼接字符串
来源：http://wap.fanxiaobao.xyz/Article/details/glpnrzcvb.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.fanxiaobao.xyz/Article/details/ggmzwesua.sHtML

[S18] C：命令行参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcazaurex.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqmxdxnsz.sHtML

[S19] C：快速排序
来源：http://3g.fanxiaobao.xyz/Article/details/gygrkpumg.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.fanxiaobao.xyz/Article/details/grphhgchq.sHtML

[S20] C：二分查找
来源：http://www.share.fanxiaobao.xyz/Article/details/grunssojb.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.fanxiaobao.xyz/Article/details/gwintqiok.sHtML

[S21] C：字符类别判断
来源：http://mobile.fanxiaobao.xyz/Article/details/gicsvlrjd.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.fanxiaobao.xyz/Article/details/gzrtrnvnw.sHtML

[S22] C：字符串转数字
来源：http://www.blog.fanxiaobao.xyz/Article/details/gciwusqcj.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.fanxiaobao.xyz/Article/details/gdcvcgsfb.sHtML

[S23] C：随机数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpzmjcizx.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.fanxiaobao.xyz/Article/details/gtafpjkng.sHtML

[S24] C：获取本地时间
来源：http://www.share.fanxiaobao.xyz/Article/details/gpdpqafcn.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.fanxiaobao.xyz/Article/details/gznupdlyn.sHtML

[S25] C：内存拷贝
来源：http://mobile.fanxiaobao.xyz/Article/details/grmuzfihm.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gioxiltdb.sHtML

[S26] C：内存清零
来源：http://3g.fanxiaobao.xyz/Article/details/gpzilugll.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.fanxiaobao.xyz/Article/details/gthvtgvcg.sHtML

[S27] C：定义常量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfnkqedmf.sHtML

const double PI = 3.14159;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqhvxxwol.sHtML

[S28] C：静态变量
来源：http://baike.fanxiaobao.xyz/Article/details/gugbgiaeq.sHtML

static int counter = 0;
来源：http://read.share.fanxiaobao.xyz/Article/details/gcukpnbor.sHtML

[S29] C：变参函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gossiacql.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.fanxiaobao.xyz/Article/details/gsayvqsyr.sHtML

[S30] C：头文件保护
来源：http://3g.fanxiaobao.xyz/Article/details/gmcbmwemb.sHtML

#ifndef X_H
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmtzugxhk.sHtML

#define X_H
来源：http://m.share.fanxiaobao.xyz/Article/details/gusaycsia.sHtML

#endif
来源：http://read.share.fanxiaobao.xyz/Article/details/gpnqwplgr.sHtML

[S31] C++：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnjmgwepr.sHtML

#include <iostream>
来源：http://www.share.fanxiaobao.xyz/Article/details/giadwidip.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.fanxiaobao.xyz/Article/details/gyzquwqsp.sHtML

[S32] C++：字符串
来源：http://mobile.fanxiaobao.xyz/Article/details/gdemkwlaj.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.fanxiaobao.xyz/Article/details/gjowmzbhx.sHtML

[S33] C++：vector 增删
来源：http://m.share.fanxiaobao.xyz/Article/details/gppvqovyx.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.fanxiaobao.xyz/Article/details/gmbmoexmu.sHtML

[S34] C++：遍历 vector
来源：http://baike.fanxiaobao.xyz/Article/details/gljqcmdic.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghbnqpxtq.sHtML

[S35] C++：map
来源：http://3g.fanxiaobao.xyz/Article/details/gyhtvqufr.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gearrguqo.sHtML

[S36] C++：unordered_map
来源：http://www.share.fanxiaobao.xyz/Article/details/gmkourykr.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.fanxiaobao.xyz/Article/details/gyvdozekl.sHtML

[S37] C++：set
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwnqibjmn.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.fanxiaobao.xyz/Article/details/gwpwsbzwo.sHtML

[S38] C++：排序
来源：http://blog.fanxiaobao.xyz/Article/details/gwttnhjas.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.fanxiaobao.xyz/Article/details/getnyvdei.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.fanxiaobao.xyz/Article/details/gopyssabg.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.fanxiaobao.xyz/Article/details/gnzsyidfh.sHtML

[S40] C++：查找元素
来源：http://m.share.fanxiaobao.xyz/Article/details/ghkaomwbt.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.fanxiaobao.xyz/Article/details/gzbmjdikm.sHtML

[S41] C++：类与构造函数
来源：http://wap.fanxiaobao.xyz/Article/details/gmcwcfhst.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.fanxiaobao.xyz/Article/details/gbybovnqg.sHtML

[S42] C++：继承与虚函数
来源：http://blog.fanxiaobao.xyz/Article/details/grbyrqhzu.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.fanxiaobao.xyz/Article/details/gymgkhnfw.sHtML

[S43] C++：智能指针
来源：http://www.share.fanxiaobao.xyz/Article/details/gwkmozzgu.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvjazznjr.sHtML

[S44] C++：引用传参
来源：http://www.share.fanxiaobao.xyz/Article/details/gztlznpkt.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbqtkkmfv.sHtML

[S45] C++：lambda
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwczsyjgp.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.fanxiaobao.xyz/Article/details/gqpexsnyd.sHtML

[S46] C++：函数模板
来源：http://read.share.fanxiaobao.xyz/Article/details/gdnonvcfn.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbqgbrwqu.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpfbpoogj.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gzifblqow.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzhrdwpvb.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghjdaywvl.sHtML

while (std::getline(in, line)) { }
来源：http://blog.fanxiaobao.xyz/Article/details/gxjnztmqb.sHtML

[S49] C++：写文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gznajrvyt.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.fanxiaobao.xyz/Article/details/gdfmcbkcx.sHtML

[S50] C++：格式化数字
来源：http://read.share.fanxiaobao.xyz/Article/details/gpbpjbyqw.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gymqdduhg.sHtML

[S51] C++：显式类型转换
来源：http://read.share.fanxiaobao.xyz/Article/details/gluiqmprt.sHtML

static_cast<double>(a) / b
来源：http://mobile.fanxiaobao.xyz/Article/details/gfieckpqx.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.fanxiaobao.xyz/Article/details/geahbbmft.sHtML

int size() const noexcept { return n_; }
来源：http://baike.fanxiaobao.xyz/Article/details/gmimqnihp.sHtML

[S53] C++：移动语义
来源：http://mobile.fanxiaobao.xyz/Article/details/goxhxrstq.sHtML

std::vector<int> w = std::move(v);
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghjgkspua.sHtML

[S54] C++：异常处理
来源：http://wap.fanxiaobao.xyz/Article/details/glwsifqoi.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtwdedcbb.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsrlnnnyb.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.fanxiaobao.xyz/Article/details/ghkommmni.sHtML

[S56] C++：optional
来源：http://3g.fanxiaobao.xyz/Article/details/gzxkzmwwc.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.fanxiaobao.xyz/Article/details/ghxecupeu.sHtML

[S57] C++：编译期常量
来源：http://m.share.fanxiaobao.xyz/Article/details/gjbozzsbk.sHtML

constexpr int N = 10;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxzoemukp.sHtML

[S58] C++：命名空间
来源：http://baike.fanxiaobao.xyz/Article/details/gqxpwvjqw.sHtML


<!-- 参考信息 -->