代发 wailian999

[Q86] 读取 JSON 字段
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdyllnmbk.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://blog.fanxiaobao.xyz/Article/details/gbrltkatj.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.fanxiaobao.xyz/Article/details/gvczvzgit.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.fanxiaobao.xyz/Article/details/gwnugswgj.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.fanxiaobao.xyz/Article/details/gqpfphbye.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.fanxiaobao.xyz/Article/details/gsitqtlas.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/geqtltsho.sHtML

[Q89] 判断表是否存在
来源：http://read.share.fanxiaobao.xyz/Article/details/ggqykikfq.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.fanxiaobao.xyz/Article/details/gcgnnfpjy.sHtML

[Q90] 生成序号列
来源：http://m.share.fanxiaobao.xyz/Article/details/ghkqeeueq.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://baike.fanxiaobao.xyz/Article/details/ggywhmjrl.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gbkoqzzkj.sHtML

R. Bash 专题
来源：http://3g.fanxiaobao.xyz/Article/details/gqjkpksxs.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gywkpcbjv.sHtML

[R01] shebang 与严格模式
来源：http://mobile.fanxiaobao.xyz/Article/details/ganyzmgcr.sHtML

#!/usr/bin/env bash
来源：http://wap.fanxiaobao.xyz/Article/details/gmwdohyty.sHtML

set -euo pipefail
来源：http://read.share.fanxiaobao.xyz/Article/details/glqmeqfto.sHtML

[R02] 变量赋值与使用
来源：http://read.share.fanxiaobao.xyz/Article/details/gzhzjuoyb.sHtML

name="Tom"; echo "$name"
来源：http://read.share.fanxiaobao.xyz/Article/details/gbohfvsuc.sHtML

[R03] 只读变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gfrbvkqsp.sHtML

readonly PI=3.14
来源：http://read.share.fanxiaobao.xyz/Article/details/geomfkcpx.sHtML

[R04] 位置参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnrllmryc.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaqyhxwdr.sHtML

[R05] 参数默认值
来源：http://baike.fanxiaobao.xyz/Article/details/gwxruwpgb.sHtML

name="${1:-default}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gqrlmzxby.sHtML

[R06] 判断命令是否存在
来源：http://blog.fanxiaobao.xyz/Article/details/gtsoyslyu.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.fanxiaobao.xyz/Article/details/geixbgbwm.sHtML

[R07] if 判断文件
来源：http://3g.fanxiaobao.xyz/Article/details/gtofxjrgf.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.fanxiaobao.xyz/Article/details/gmpdktevl.sHtML

[R08] 数值比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/goivehszl.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.fanxiaobao.xyz/Article/details/gahdqxaro.sHtML

[R09] 字符串比较
来源：http://baike.fanxiaobao.xyz/Article/details/gnijorypr.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.fanxiaobao.xyz/Article/details/gqsivslzi.sHtML

[R10] 正则匹配
来源：http://m.share.fanxiaobao.xyz/Article/details/ghbaayiiz.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.fanxiaobao.xyz/Article/details/gbhwjotnx.sHtML

[R11] case 多分支
来源：http://m.share.fanxiaobao.xyz/Article/details/gmimmiwbg.sHtML

case "$1" in
来源：http://wap.fanxiaobao.xyz/Article/details/gdghgxlyi.sHtML

start) echo "启动" ;;
来源：http://mobile.fanxiaobao.xyz/Article/details/gtxqnqlzh.sHtML

stop)  echo "停止" ;;
来源：http://3g.fanxiaobao.xyz/Article/details/gewezxizt.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.fanxiaobao.xyz/Article/details/gyawsgxzj.sHtML

esac
来源：http://mobile.fanxiaobao.xyz/Article/details/gckwwvpnr.sHtML

[R12] for 遍历文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gmnlrmqno.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpdjbqiuq.sHtML

[R13] for 计数循环
来源：http://3g.fanxiaobao.xyz/Article/details/gjivyhwsi.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gxuqaukpw.sHtML

[R14] C 风格 for
来源：http://mobile.fanxiaobao.xyz/Article/details/grhgkuaxb.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.fanxiaobao.xyz/Article/details/gufwvmkdd.sHtML

[R15] while 逐行读文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gtkxhaibr.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gfggmhamv.sHtML

[R16] until 等待条件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gscjcwopj.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.fanxiaobao.xyz/Article/details/geuuxkoqf.sHtML

[R17] 数组定义与取值
来源：http://blog.fanxiaobao.xyz/Article/details/gslwlpcjp.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gaishabfc.sHtML

[R18] 遍历数组
来源：http://baike.fanxiaobao.xyz/Article/details/gvndtbejf.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.fanxiaobao.xyz/Article/details/gqtyuzpus.sHtML

[R19] 数组长度
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjfkfcbjy.sHtML

echo "${#arr[@]}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gmedamqpn.sHtML

[R20] 关联数组（字典）
来源：http://mobile.fanxiaobao.xyz/Article/details/gdrcvsysu.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gefxxmsaz.sHtML

[R21] 字符串长度
来源：http://mobile.fanxiaobao.xyz/Article/details/ghttdpjlx.sHtML

echo "${#s}"
来源：http://blog.fanxiaobao.xyz/Article/details/gtfbelzhj.sHtML

[R22] 截取子串
来源：http://blog.fanxiaobao.xyz/Article/details/gyhzkzdfo.sHtML

echo "${s:0:5}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gughtnbfr.sHtML

[R23] 字符串替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gijcnlftx.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.fanxiaobao.xyz/Article/details/gizqkpbep.sHtML

[R24] 大小写转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwgvjzvae.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.fanxiaobao.xyz/Article/details/gpchnvnxg.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.fanxiaobao.xyz/Article/details/gydhtsoht.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gtzghidqi.sHtML

[R26] 命令替换
来源：http://3g.fanxiaobao.xyz/Article/details/gqtuqgsgx.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.fanxiaobao.xyz/Article/details/ghnygsehz.sHtML

[R27] 算术展开
来源：http://www.share.fanxiaobao.xyz/Article/details/gnelnnnur.sHtML

echo $((1 + 2 * 3))
来源：http://3g.fanxiaobao.xyz/Article/details/gmrrlrsmk.sHtML

[R28] 浮点运算
来源：http://mobile.fanxiaobao.xyz/Article/details/gowogmfte.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.fanxiaobao.xyz/Article/details/gvameyfoy.sHtML

[R29] 定义函数
来源：http://mobile.fanxiaobao.xyz/Article/details/galaogbdg.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/gceshndso.sHtML

[R30] 函数返回状态码
来源：http://www.blog.fanxiaobao.xyz/Article/details/gffeogswg.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.fanxiaobao.xyz/Article/details/gblnmxqya.sHtML

[R31] 局部变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvmhmsydh.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzkqykyrb.sHtML

[R32] 参数个数校验
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwuhtbysm.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmtmevesg.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.fanxiaobao.xyz/Article/details/guanjnrjc.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.fanxiaobao.xyz/Article/details/gptdideed.sHtML

[R34] 退出时清理
来源：http://m.share.fanxiaobao.xyz/Article/details/gzqxnfpes.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.fanxiaobao.xyz/Article/details/grptyqmnk.sHtML

[R35] 后台执行并等待
来源：http://wap.fanxiaobao.xyz/Article/details/gcczossdt.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvkacwipj.sHtML

[R36] 并发执行多个任务
来源：http://3g.fanxiaobao.xyz/Article/details/gemhyobii.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.fanxiaobao.xyz/Article/details/gysqwcuse.sHtML

[R37] 把输出赋给变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gqxzlswot.sHtML

files=$(ls -1)
来源：http://wap.fanxiaobao.xyz/Article/details/gkkggyzib.sHtML

[R38] 管道串联
来源：http://3g.fanxiaobao.xyz/Article/details/gdjewtckb.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.fanxiaobao.xyz/Article/details/gklhnwvbc.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.fanxiaobao.xyz/Article/details/glfuayqyk.sHtML

cmd > out.log 2>&1
来源：http://wap.fanxiaobao.xyz/Article/details/gqdrsatyd.sHtML

[R40] 追加写日志
来源：http://read.share.fanxiaobao.xyz/Article/details/gzuwaablg.sHtML

echo "log" >> out.log
来源：http://read.share.fanxiaobao.xyz/Article/details/gpapbvwqv.sHtML

[R41] 丢弃输出
来源：http://wap.fanxiaobao.xyz/Article/details/gzfcgmegn.sHtML

cmd >/dev/null 2>&1
来源：http://wap.fanxiaobao.xyz/Article/details/gtvrqhqgo.sHtML

[R42] 输入重定向
来源：http://www.share.fanxiaobao.xyz/Article/details/gieegduqs.sHtML

wc -l < a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gibynaeic.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gemvngoze.sHtML

find . -name "*.log" -type f
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzjubmvwe.sHtML

[R44] 按修改时间查找
来源：http://baike.fanxiaobao.xyz/Article/details/ggxmcljno.sHtML

find . -mtime -7 -type f
来源：http://read.share.fanxiaobao.xyz/Article/details/gubiqrumf.sHtML

[R45] 批量删除
来源：http://m.share.fanxiaobao.xyz/Article/details/gtuwfentm.sHtML

find . -name "*.tmp" -delete
来源：http://baike.fanxiaobao.xyz/Article/details/gnbknpuqd.sHtML

[R46] 递归替换文件内容
来源：http://baike.fanxiaobao.xyz/Article/details/gxetdbnhd.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.fanxiaobao.xyz/Article/details/grrwcalhk.sHtML

[R47] sed 单行替换
来源：http://wap.fanxiaobao.xyz/Article/details/guswhsvwv.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/ggtarazgi.sHtML

[R48] awk 取指定列
来源：http://baike.fanxiaobao.xyz/Article/details/gbtltbayq.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gsdcrsdjd.sHtML

[R49] awk 带条件
来源：http://3g.fanxiaobao.xyz/Article/details/glvmbclev.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.fanxiaobao.xyz/Article/details/gkykcukfx.sHtML

[R50] awk 求和
来源：http://m.share.fanxiaobao.xyz/Article/details/gtilpazhp.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gohsvmnbi.sHtML

[R51] 排序去重取前几
来源：http://baike.fanxiaobao.xyz/Article/details/gspgmiusm.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.fanxiaobao.xyz/Article/details/gjfczqapb.sHtML

[R52] 统计行数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghyfuzsgz.sHtML

wc -l a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gigraxyqs.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.fanxiaobao.xyz/Article/details/gfasflimc.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.fanxiaobao.xyz/Article/details/gbfncfama.sHtML

[R54] 比较两个文件
来源：http://wap.fanxiaobao.xyz/Article/details/gvbxkkjdg.sHtML

diff a.txt b.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbgjckiki.sHtML

[R55] 压缩与解压
来源：http://read.share.fanxiaobao.xyz/Article/details/gbsjocwck.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.fanxiaobao.xyz/Article/details/gblnykjlu.sHtML

[R56] 远程拷贝
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdxonbfjf.sHtML

scp file user@host:/path/
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtvzcomcz.sHtML

[R57] 远程执行命令
来源：http://3g.fanxiaobao.xyz/Article/details/gzzjobonk.sHtML

ssh user@host 'uptime'
来源：http://3g.fanxiaobao.xyz/Article/details/gvgbbejkl.sHtML

[R58] 下载文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gempymnrg.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.fanxiaobao.xyz/Article/details/guqazmooi.sHtML

[R59] 发 POST JSON
来源：http://read.share.fanxiaobao.xyz/Article/details/ghxjfiyob.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grhprivwl.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfquwlktg.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.fanxiaobao.xyz/Article/details/gtquqpsfz.sHtML

[R61] 磁盘占用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzbzfxhsu.sHtML

df -h;  du -sh *
来源：http://mobile.fanxiaobao.xyz/Article/details/gokfvrzpq.sHtML

[R62] 找最占空间的文件
来源：http://wap.fanxiaobao.xyz/Article/details/gcorotsec.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.fanxiaobao.xyz/Article/details/gmkgimhct.sHtML

[R63] 内存与进程
来源：http://mobile.fanxiaobao.xyz/Article/details/gmgosnblc.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.fanxiaobao.xyz/Article/details/gpavcmfzy.sHtML

[R64] 结束进程
来源：http://3g.fanxiaobao.xyz/Article/details/glcxxwzwp.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggxexvbte.sHtML

[R65] 查看端口占用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvtdsatas.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.fanxiaobao.xyz/Article/details/gzuajuksk.sHtML

[R66] 定时任务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giseehsaw.sHtML

crontab -e;  crontab -l
来源：http://blog.fanxiaobao.xyz/Article/details/gfnyraqdp.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.fanxiaobao.xyz/Article/details/ggvlcbyov.sHtML

openssl rand -hex 16
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gymjpiqyh.sHtML

[R68] 计算文件校验值
来源：http://read.share.fanxiaobao.xyz/Article/details/ghdhqrwij.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gqyuauyzz.sHtML

[R69] 生成随机密码
来源：http://baike.fanxiaobao.xyz/Article/details/gtibrczfb.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.fanxiaobao.xyz/Article/details/glxjvuqmg.sHtML

[R70] 时间戳与互转
来源：http://read.share.fanxiaobao.xyz/Article/details/gwaecfxgc.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggtvkshez.sHtML

[R71] 日期格式化
来源：http://m.share.fanxiaobao.xyz/Article/details/guhmhukif.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gauqkyioy.sHtML

[R72] 等待端口就绪
来源：http://baike.fanxiaobao.xyz/Article/details/gexemumlt.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gkkycwbpf.sHtML

[R73] 分割大日志
来源：http://wap.fanxiaobao.xyz/Article/details/gbjthtklq.sHtML

split -l 1000 big.log part_
来源：http://baike.fanxiaobao.xyz/Article/details/gexlciyzg.sHtML

[R74] 批量重命名
来源：http://blog.fanxiaobao.xyz/Article/details/getbvumdy.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gufacgzzj.sHtML

[R75] 导出环境变量
来源：http://baike.fanxiaobao.xyz/Article/details/gentzqugn.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.fanxiaobao.xyz/Article/details/gmqafnxtn.sHtML

[R76] 使用临时文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzwlpgvgb.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.fanxiaobao.xyz/Article/details/gctjehfdw.sHtML

[R77] 读取用户输入
来源：http://3g.fanxiaobao.xyz/Article/details/gsebfnqhi.sHtML

read -rp "请输入: " ans
来源：http://blog.fanxiaobao.xyz/Article/details/gdmsdauax.sHtML

[R78] 交互式菜单
来源：http://mobile.fanxiaobao.xyz/Article/details/gekidvjwo.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gbuwicsrr.sHtML

[R79] 解析命令行选项
来源：http://baike.fanxiaobao.xyz/Article/details/gbjmvsdvx.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpkaygtcc.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.fanxiaobao.xyz/Article/details/gqepuijma.sHtML

time ./run.sh
来源：http://read.share.fanxiaobao.xyz/Article/details/gysnuorha.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gcuiekaia.sHtML

S. C / C++ 专题
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grtwuhlpl.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggtgbrtop.sHtML

[S01] C：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gkveztqts.sHtML

#include <stdio.h>
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnfwbvjpj.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbrzfhaaq.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.fanxiaobao.xyz/Article/details/gaphdqqnd.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxqvszigg.sHtML

[S03] C：读入整数
来源：http://www.share.fanxiaobao.xyz/Article/details/gfmawmfyf.sHtML

int x; scanf("%d", &x);
来源：http://3g.fanxiaobao.xyz/Article/details/glcqjukty.sHtML

[S04] C：字符串复制
来源：http://3g.fanxiaobao.xyz/Article/details/gbnkwkwdm.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.fanxiaobao.xyz/Article/details/grsoatkzh.sHtML

[S05] C：字符串长度
来源：http://www.share.fanxiaobao.xyz/Article/details/gufulgbok.sHtML

strlen(s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmiljrelt.sHtML

[S06] C：字符串比较
来源：http://baike.fanxiaobao.xyz/Article/details/ghewbnelr.sHtML

strcmp(a, b) == 0
来源：http://www.blog.fanxiaobao.xyz/Article/details/gteoeqyvl.sHtML

[S07] C：数组遍历求和
来源：http://wap.fanxiaobao.xyz/Article/details/gdmhefuvx.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.fanxiaobao.xyz/Article/details/glegflsys.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.fanxiaobao.xyz/Article/details/gkgfitkxj.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.fanxiaobao.xyz/Article/details/gnqbxpujg.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.fanxiaobao.xyz/Article/details/gensebtwe.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.fanxiaobao.xyz/Article/details/gjttxeemr.sHtML

[S10] C：指针与解引用
来源：http://m.share.fanxiaobao.xyz/Article/details/gndukrdte.sHtML

int *p = &a;  *p = 5;
来源：http://wap.fanxiaobao.xyz/Article/details/gwurpiuoa.sHtML

[S11] C：逐行读文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqitwpvgi.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.fanxiaobao.xyz/Article/details/ggudiqqdl.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.fanxiaobao.xyz/Article/details/gpkaciomf.sHtML

fclose(f);
来源：http://3g.fanxiaobao.xyz/Article/details/gksvzesmb.sHtML

[S12] C：写文件
来源：http://3g.fanxiaobao.xyz/Article/details/ggxqxbvnt.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.fanxiaobao.xyz/Article/details/gvasirfwi.sHtML

[S13] C：宏定义
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggjghpggu.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.fanxiaobao.xyz/Article/details/gjayvjaos.sHtML

[S14] C：枚举
来源：http://3g.fanxiaobao.xyz/Article/details/gtmbjlknz.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gssemlcjs.sHtML

[S15] C：类型转换
来源：http://read.share.fanxiaobao.xyz/Article/details/gnnqnitlj.sHtML

(double) a / b
来源：http://baike.fanxiaobao.xyz/Article/details/gzwlyvvnk.sHtML

[S16] C：位操作置位
来源：http://m.share.fanxiaobao.xyz/Article/details/gfevevgug.sHtML

x |= (1 << 3);
来源：http://blog.fanxiaobao.xyz/Article/details/gcxxkcoyg.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.fanxiaobao.xyz/Article/details/gmzcvkmhn.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.fanxiaobao.xyz/Article/details/gssaekrvu.sHtML

[S18] C：命令行参数
来源：http://3g.fanxiaobao.xyz/Article/details/gyfjfdefv.sHtML

int main(int argc, char **argv)
来源：http://mobile.fanxiaobao.xyz/Article/details/gihpqqlvi.sHtML

[S19] C：快速排序
来源：http://3g.fanxiaobao.xyz/Article/details/gquqzqcmt.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.fanxiaobao.xyz/Article/details/gtixjpqnb.sHtML

[S20] C：二分查找
来源：http://read.share.fanxiaobao.xyz/Article/details/gqvchecdn.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.fanxiaobao.xyz/Article/details/gwywinhkh.sHtML

[S21] C：字符类别判断
来源：http://mobile.fanxiaobao.xyz/Article/details/gipzegcvv.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gktpwinrn.sHtML

[S22] C：字符串转数字
来源：http://3g.fanxiaobao.xyz/Article/details/gmijmqdno.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.fanxiaobao.xyz/Article/details/gwtgfsqbg.sHtML

[S23] C：随机数
来源：http://baike.fanxiaobao.xyz/Article/details/gwdiwkmoa.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvnlgpudq.sHtML

[S24] C：获取本地时间
来源：http://mobile.fanxiaobao.xyz/Article/details/gabdgrslr.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.fanxiaobao.xyz/Article/details/gsjaeegfx.sHtML

[S25] C：内存拷贝
来源：http://3g.fanxiaobao.xyz/Article/details/gyxfkmyxg.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqpnebmuj.sHtML

[S26] C：内存清零
来源：http://mobile.fanxiaobao.xyz/Article/details/gdtwofuvn.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.fanxiaobao.xyz/Article/details/gldrfvolr.sHtML

[S27] C：定义常量
来源：http://3g.fanxiaobao.xyz/Article/details/gmetyvwav.sHtML

const double PI = 3.14159;
来源：http://www.share.fanxiaobao.xyz/Article/details/gcpqwpkog.sHtML

[S28] C：静态变量
来源：http://3g.fanxiaobao.xyz/Article/details/gpokujrle.sHtML

static int counter = 0;
来源：http://m.share.fanxiaobao.xyz/Article/details/gwiybxpws.sHtML

[S29] C：变参函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gtukbzlwl.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.fanxiaobao.xyz/Article/details/geqhjcbrd.sHtML

[S30] C：头文件保护
来源：http://wap.fanxiaobao.xyz/Article/details/gdpjnqmos.sHtML

#ifndef X_H
来源：http://mobile.fanxiaobao.xyz/Article/details/gcopgoolw.sHtML

#define X_H
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvwmhlany.sHtML

#endif
来源：http://www.share.fanxiaobao.xyz/Article/details/gghjgfgsz.sHtML

[S31] C++：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gypyyqnbs.sHtML

#include <iostream>
来源：http://mobile.fanxiaobao.xyz/Article/details/gqbguqlhc.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gotngjvky.sHtML

[S32] C++：字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/gbymiqmac.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.fanxiaobao.xyz/Article/details/gqdjlpahq.sHtML

[S33] C++：vector 增删
来源：http://wap.fanxiaobao.xyz/Article/details/gxjismftr.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.fanxiaobao.xyz/Article/details/gkduenhcy.sHtML

[S34] C++：遍历 vector
来源：http://3g.fanxiaobao.xyz/Article/details/gtjlgnmbo.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.fanxiaobao.xyz/Article/details/gckbpqxzy.sHtML

[S35] C++：map
来源：http://blog.fanxiaobao.xyz/Article/details/gapxkcimm.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fanxiaobao.xyz/Article/details/gkmxggmdl.sHtML

[S36] C++：unordered_map
来源：http://baike.fanxiaobao.xyz/Article/details/gbhvxvura.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fanxiaobao.xyz/Article/details/gfyqdxitp.sHtML

[S37] C++：set
来源：http://wap.fanxiaobao.xyz/Article/details/gnwogauom.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.fanxiaobao.xyz/Article/details/gnxaxtkjr.sHtML

[S38] C++：排序
来源：http://3g.fanxiaobao.xyz/Article/details/gvhckwdka.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.fanxiaobao.xyz/Article/details/gidssumcf.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.fanxiaobao.xyz/Article/details/gvkdebmhf.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.fanxiaobao.xyz/Article/details/gbyjgusnc.sHtML

[S40] C++：查找元素
来源：http://read.share.fanxiaobao.xyz/Article/details/gothvdoaq.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.fanxiaobao.xyz/Article/details/gqbqwkive.sHtML

[S41] C++：类与构造函数
来源：http://blog.fanxiaobao.xyz/Article/details/grzdfvhhn.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.fanxiaobao.xyz/Article/details/gwuychrpm.sHtML

[S42] C++：继承与虚函数
来源：http://baike.fanxiaobao.xyz/Article/details/gkupopwas.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.fanxiaobao.xyz/Article/details/gslbndrjq.sHtML

[S43] C++：智能指针
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghxufhtse.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.fanxiaobao.xyz/Article/details/guihfjzdv.sHtML

[S44] C++：引用传参
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnhddswwk.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.fanxiaobao.xyz/Article/details/ghtvuujly.sHtML

[S45] C++：lambda
来源：http://baike.fanxiaobao.xyz/Article/details/gfaserfil.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.fanxiaobao.xyz/Article/details/giebnpqgh.sHtML

[S46] C++：函数模板
来源：http://m.share.fanxiaobao.xyz/Article/details/gekjkwyyh.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gmbonybam.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.fanxiaobao.xyz/Article/details/gsxastccr.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/guwffrvsd.sHtML

[S48] C++：逐行读文件
来源：http://blog.fanxiaobao.xyz/Article/details/gkhrattbi.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gslkwotrj.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.fanxiaobao.xyz/Article/details/gugwuxhyu.sHtML

[S49] C++：写文件
来源：http://wap.fanxiaobao.xyz/Article/details/gschcnvhu.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.fanxiaobao.xyz/Article/details/gmjzixegm.sHtML

[S50] C++：格式化数字
来源：http://read.share.fanxiaobao.xyz/Article/details/gicttfqrd.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.fanxiaobao.xyz/Article/details/gcjsfkmwq.sHtML

[S51] C++：显式类型转换
来源：http://baike.fanxiaobao.xyz/Article/details/ggqtvzcyj.sHtML

static_cast<double>(a) / b
来源：http://www.blog.fanxiaobao.xyz/Article/details/gasezoexw.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gypyjiycb.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gahfhqsqk.sHtML

[S53] C++：移动语义
来源：http://blog.fanxiaobao.xyz/Article/details/gqnskakhd.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.fanxiaobao.xyz/Article/details/gbtkfbhdz.sHtML

[S54] C++：异常处理
来源：http://wap.fanxiaobao.xyz/Article/details/gmxusjrkr.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.fanxiaobao.xyz/Article/details/gxeugeztk.sHtML

[S55] C++：结构化绑定
来源：http://www.share.fanxiaobao.xyz/Article/details/gdbzmfpyb.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.fanxiaobao.xyz/Article/details/gxdvjcqxt.sHtML

[S56] C++：optional
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzdixbuqm.sHtML


<!-- 参考信息 -->