代发 wailian999

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.fehbvm.com/Article/details/gcvxcpnbz.sHtML

[Q90] 生成序号列
来源：http://blog.hesvh.cn/Article/details/gqayvporn.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://baike.hesvh.cn/Article/details/gypfxxtvp.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gfwfgypkl.sHtML

R. Bash 专题
来源：http://www.m.share.fehbvm.com/Article/details/gzwfeeysr.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gsxkxtfgz.sHtML

[R01] shebang 与严格模式
来源：http://3g.zdbjq.cn/Article/details/glensbxum.sHtML

#!/usr/bin/env bash
来源：http://m.share.fehbvm.com/Article/details/gkqzdslqn.sHtML

set -euo pipefail
来源：http://3g.hesvh.cn/Article/details/gzhoricll.sHtML

[R02] 变量赋值与使用
来源：http://mobile.hesvh.cn/Article/details/gqjcajyko.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.hesvh.cn/Article/details/gvssgmeqq.sHtML

[R03] 只读变量
来源：http://www.share.fehbvm.com/Article/details/gcezzcrjl.sHtML

readonly PI=3.14
来源：http://read.share.zdbjq.cn/Article/details/gjdqgdqnb.sHtML

[R04] 位置参数
来源：http://blog.zdbjq.cn/Article/details/gjygejqss.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.hesvh.cn/Article/details/gklfeejai.sHtML

[R05] 参数默认值
来源：http://www.m.share.zdbjq.cn/Article/details/gfaihtuee.sHtML

name="${1:-default}"
来源：http://www.blog.fehbvm.com/Article/details/gjwonlyyi.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.fehbvm.com/Article/details/gsvmyppxh.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.zdbjq.cn/Article/details/gimwajnas.sHtML

[R07] if 判断文件
来源：http://3g.zdbjq.cn/Article/details/gwxnzynzi.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.hesvh.cn/Article/details/gcwmmanns.sHtML

[R08] 数值比较
来源：http://wap.fehbvm.com/Article/details/gzhklsowp.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.fehbvm.com/Article/details/gffgvqyeg.sHtML

[R09] 字符串比较
来源：http://blog.zdbjq.cn/Article/details/gzzhykzoa.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.hesvh.cn/Article/details/gfljiowqt.sHtML

[R10] 正则匹配
来源：http://blog.fehbvm.com/Article/details/geubpuxzc.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.fehbvm.com/Article/details/gbmgxbveh.sHtML

[R11] case 多分支
来源：http://baike.fehbvm.com/Article/details/gqlcjzmew.sHtML

case "$1" in
来源：http://3g.zdbjq.cn/Article/details/gingoroyb.sHtML

start) echo "启动" ;;
来源：http://3g.fehbvm.com/Article/details/gzzxnqawx.sHtML

stop)  echo "停止" ;;
来源：http://3g.fehbvm.com/Article/details/gllrkdcfq.sHtML

*)     echo "未知命令" ;;
来源：http://www.share.hesvh.cn/Article/details/gnzllfbum.sHtML

esac
来源：http://wap.zdbjq.cn/Article/details/gmlqrhjod.sHtML

[R12] for 遍历文件
来源：http://mobile.fehbvm.com/Article/details/gllmzkklx.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.hesvh.cn/Article/details/geyomdxyq.sHtML

[R13] for 计数循环
来源：http://blog.hesvh.cn/Article/details/gmgxvfsoy.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.fehbvm.com/Article/details/gmjrgyhmu.sHtML

[R14] C 风格 for
来源：http://wap.zdbjq.cn/Article/details/gtckoebdu.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.fehbvm.com/Article/details/gyjwtujux.sHtML

[R15] while 逐行读文件
来源：http://baike.hesvh.cn/Article/details/gmjnydmoe.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.fehbvm.com/Article/details/guxahrjpo.sHtML

[R16] until 等待条件
来源：http://baike.hesvh.cn/Article/details/gvtzwgfyd.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.share.zdbjq.cn/Article/details/gdiqezqnv.sHtML

[R17] 数组定义与取值
来源：http://read.share.zdbjq.cn/Article/details/gymjdwtsr.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://3g.fehbvm.com/Article/details/gwkaehgiv.sHtML

[R18] 遍历数组
来源：http://baike.fehbvm.com/Article/details/gpyqvjmwf.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.m.share.fehbvm.com/Article/details/giotjpoyj.sHtML

[R19] 数组长度
来源：http://blog.hesvh.cn/Article/details/gtoxbfxde.sHtML

echo "${#arr[@]}"
来源：http://3g.zdbjq.cn/Article/details/gayxjisnk.sHtML

[R20] 关联数组（字典）
来源：http://baike.zdbjq.cn/Article/details/gzndzdcom.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mobile.fehbvm.com/Article/details/gmjeetxwo.sHtML

[R21] 字符串长度
来源：http://3g.hesvh.cn/Article/details/gyefxfnqj.sHtML

echo "${#s}"
来源：http://wap.hesvh.cn/Article/details/gyokcfvee.sHtML

[R22] 截取子串
来源：http://3g.zdbjq.cn/Article/details/gsflenwyi.sHtML

echo "${s:0:5}"
来源：http://m.share.fehbvm.com/Article/details/guaykbspg.sHtML

[R23] 字符串替换
来源：http://blog.zdbjq.cn/Article/details/gmtsavumk.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.zdbjq.cn/Article/details/gcgbgvcji.sHtML

[R24] 大小写转换
来源：http://www.blog.zdbjq.cn/Article/details/gcaafucma.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.fehbvm.com/Article/details/geuklzyxy.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.hesvh.cn/Article/details/geplzywks.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.hesvh.cn/Article/details/gmetofutr.sHtML

[R26] 命令替换
来源：http://m.share.fehbvm.com/Article/details/gnlnervyf.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.zdbjq.cn/Article/details/gavcyetgo.sHtML

[R27] 算术展开
来源：http://baike.zdbjq.cn/Article/details/gsoweubxs.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.fehbvm.com/Article/details/gtztuvumj.sHtML

[R28] 浮点运算
来源：http://3g.hesvh.cn/Article/details/gdwljuwuy.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.hesvh.cn/Article/details/gtwjcmqmh.sHtML

[R29] 定义函数
来源：http://m.share.fehbvm.com/Article/details/gceygpczk.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.hesvh.cn/Article/details/gynykkchm.sHtML

[R30] 函数返回状态码
来源：http://m.share.hesvh.cn/Article/details/guccqqlik.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.fehbvm.com/Article/details/gfaqfxnwt.sHtML

[R31] 局部变量
来源：http://read.share.fehbvm.com/Article/details/ghxbdnwmq.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.hesvh.cn/Article/details/gsjkdhmjc.sHtML

[R32] 参数个数校验
来源：http://www.blog.fehbvm.com/Article/details/gyyjughaa.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.fehbvm.com/Article/details/gwtufubiq.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.fehbvm.com/Article/details/grzkrjkpu.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.zdbjq.cn/Article/details/gdzybwoyu.sHtML

[R34] 退出时清理
来源：http://m.share.zdbjq.cn/Article/details/gamewnndf.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fehbvm.com/Article/details/gdwmzxodq.sHtML

[R35] 后台执行并等待
来源：http://wap.hesvh.cn/Article/details/gsjssojcx.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.zdbjq.cn/Article/details/ggqvuxkcg.sHtML

[R36] 并发执行多个任务
来源：http://blog.fehbvm.com/Article/details/gjxdeypml.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.fehbvm.com/Article/details/gspnhqtab.sHtML

[R37] 把输出赋给变量
来源：http://mobile.fehbvm.com/Article/details/gkpkvasep.sHtML

files=$(ls -1)
来源：http://read.share.zdbjq.cn/Article/details/gwybkkjdr.sHtML

[R38] 管道串联
来源：http://mobile.hesvh.cn/Article/details/gswbldvuu.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.hesvh.cn/Article/details/gtfsbctom.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.hesvh.cn/Article/details/gzfvzkggm.sHtML

cmd > out.log 2>&1
来源：http://blog.hesvh.cn/Article/details/gkuotfxby.sHtML

[R40] 追加写日志
来源：http://wap.zdbjq.cn/Article/details/gzvkrqabh.sHtML

echo "log" >> out.log
来源：http://blog.zdbjq.cn/Article/details/gooqvnppy.sHtML

[R41] 丢弃输出
来源：http://blog.fehbvm.com/Article/details/gmzgnbcmm.sHtML

cmd >/dev/null 2>&1
来源：http://3g.fehbvm.com/Article/details/giyzwgqbc.sHtML

[R42] 输入重定向
来源：http://www.m.share.hesvh.cn/Article/details/gaeeudico.sHtML

wc -l < a.txt
来源：http://baike.zdbjq.cn/Article/details/gmundeuya.sHtML

[R43] 按名字查找文件
来源：http://blog.zdbjq.cn/Article/details/gzlroscie.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.zdbjq.cn/Article/details/gyktucakj.sHtML

[R44] 按修改时间查找
来源：http://blog.fehbvm.com/Article/details/gsoyvsuqy.sHtML

find . -mtime -7 -type f
来源：http://www.share.hesvh.cn/Article/details/gubcbhugr.sHtML

[R45] 批量删除
来源：http://baike.zdbjq.cn/Article/details/gdjgdfsop.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.zdbjq.cn/Article/details/gonovgdmr.sHtML

[R46] 递归替换文件内容
来源：http://mobile.hesvh.cn/Article/details/gzrzxnnya.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.zdbjq.cn/Article/details/gnifwnrlo.sHtML

[R47] sed 单行替换
来源：http://www.m.share.hesvh.cn/Article/details/gpjezzfxl.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.fehbvm.com/Article/details/gjpbzrwkb.sHtML

[R48] awk 取指定列
来源：http://baike.hesvh.cn/Article/details/gxstttosw.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.fehbvm.com/Article/details/gfjlvjpyh.sHtML

[R49] awk 带条件
来源：http://m.share.fehbvm.com/Article/details/gaotwxunk.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.fehbvm.com/Article/details/gaxnrzzss.sHtML

[R50] awk 求和
来源：http://wap.fehbvm.com/Article/details/goalbenro.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.fehbvm.com/Article/details/geuxrdsyb.sHtML

[R51] 排序去重取前几
来源：http://read.share.hesvh.cn/Article/details/gcmdojpba.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.hesvh.cn/Article/details/glsqaghmm.sHtML

[R52] 统计行数
来源：http://m.share.zdbjq.cn/Article/details/gvdcbisnv.sHtML

wc -l a.txt
来源：http://www.blog.zdbjq.cn/Article/details/gneuporri.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.fehbvm.com/Article/details/gvcyuived.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.hesvh.cn/Article/details/gilfyqwlw.sHtML

[R54] 比较两个文件
来源：http://www.m.share.zdbjq.cn/Article/details/gecnrvcae.sHtML

diff a.txt b.txt
来源：http://baike.hesvh.cn/Article/details/gekoomzbk.sHtML

[R55] 压缩与解压
来源：http://wap.zdbjq.cn/Article/details/gyulonfsn.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.fehbvm.com/Article/details/grlkmxzql.sHtML

[R56] 远程拷贝
来源：http://baike.zdbjq.cn/Article/details/geqhwcloc.sHtML

scp file user@host:/path/
来源：http://mobile.zdbjq.cn/Article/details/gkbhwtlad.sHtML

[R57] 远程执行命令
来源：http://www.share.zdbjq.cn/Article/details/grsmvcfkd.sHtML

ssh user@host 'uptime'
来源：http://3g.fehbvm.com/Article/details/gtjepofxl.sHtML

[R58] 下载文件
来源：http://m.share.fehbvm.com/Article/details/gcyhfkouy.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.hesvh.cn/Article/details/giofwiusl.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.zdbjq.cn/Article/details/goztugpsz.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.hesvh.cn/Article/details/gpxrbkaft.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.fehbvm.com/Article/details/gxeuwyvup.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.hesvh.cn/Article/details/gbzmknfrb.sHtML

[R61] 磁盘占用
来源：http://blog.zdbjq.cn/Article/details/gonoyetfy.sHtML

df -h;  du -sh *
来源：http://baike.fehbvm.com/Article/details/gxveeajpm.sHtML

[R62] 找最占空间的文件
来源：http://www.share.fehbvm.com/Article/details/gpmxakkns.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.hesvh.cn/Article/details/gptiqzyat.sHtML

[R63] 内存与进程
来源：http://m.share.fehbvm.com/Article/details/gdlypmspt.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.zdbjq.cn/Article/details/guapbmgkx.sHtML

[R64] 结束进程
来源：http://baike.fehbvm.com/Article/details/gjtztlwhm.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.fehbvm.com/Article/details/gdtvieckk.sHtML

[R65] 查看端口占用
来源：http://m.share.fehbvm.com/Article/details/gxnizonci.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.zdbjq.cn/Article/details/gpnbjlgrg.sHtML

[R66] 定时任务
来源：http://www.m.share.fehbvm.com/Article/details/grwuisevp.sHtML

crontab -e;  crontab -l
来源：http://m.share.zdbjq.cn/Article/details/gucktgffy.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.zdbjq.cn/Article/details/gpredxnkx.sHtML

openssl rand -hex 16
来源：http://mobile.hesvh.cn/Article/details/gxilmyrdr.sHtML

[R68] 计算文件校验值
来源：http://mobile.fehbvm.com/Article/details/gqlvpvzxr.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.zdbjq.cn/Article/details/gyjuvwzoc.sHtML

[R69] 生成随机密码
来源：http://www.m.share.fehbvm.com/Article/details/gdrnksqik.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.fehbvm.com/Article/details/gvfawaxiq.sHtML

[R70] 时间戳与互转
来源：http://baike.fehbvm.com/Article/details/giagstfgg.sHtML

date +%s;  date -d @1700000000
来源：http://baike.zdbjq.cn/Article/details/gzhumwfdi.sHtML

[R71] 日期格式化
来源：http://wap.fehbvm.com/Article/details/gesentgla.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.hesvh.cn/Article/details/gsdpfrmnv.sHtML

[R72] 等待端口就绪
来源：http://mobile.zdbjq.cn/Article/details/gyywocapb.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.fehbvm.com/Article/details/glusqkten.sHtML

[R73] 分割大日志
来源：http://baike.zdbjq.cn/Article/details/gsksgwydp.sHtML

split -l 1000 big.log part_
来源：http://www.blog.zdbjq.cn/Article/details/gyrjeshoo.sHtML

[R74] 批量重命名
来源：http://blog.hesvh.cn/Article/details/gkptpcing.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.fehbvm.com/Article/details/gjmdpmdeo.sHtML

[R75] 导出环境变量
来源：http://www.m.share.hesvh.cn/Article/details/guhpwtntr.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.hesvh.cn/Article/details/gcvzqzrod.sHtML

[R76] 使用临时文件
来源：http://read.share.zdbjq.cn/Article/details/gcmjgiqjl.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.zdbjq.cn/Article/details/gdwjcvcnf.sHtML

[R77] 读取用户输入
来源：http://3g.zdbjq.cn/Article/details/gwtidwvyf.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.hesvh.cn/Article/details/gyvjbkhhf.sHtML

[R78] 交互式菜单
来源：http://m.share.zdbjq.cn/Article/details/gpylvwwut.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.zdbjq.cn/Article/details/gruimpdcz.sHtML

[R79] 解析命令行选项
来源：http://www.share.hesvh.cn/Article/details/giqdtpoku.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.hesvh.cn/Article/details/gtjtistqn.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.zdbjq.cn/Article/details/ggxerqmua.sHtML

time ./run.sh
来源：http://www.share.hesvh.cn/Article/details/gqahimgon.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/giqcqydca.sHtML

S. C / C++ 专题
来源：http://m.share.fehbvm.com/Article/details/gvpxvxqyi.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gwtgtekyf.sHtML

[S01] C：Hello World
来源：http://baike.hesvh.cn/Article/details/ggnymthjp.sHtML

#include <stdio.h>
来源：http://mobile.fehbvm.com/Article/details/gmxvswoul.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.hesvh.cn/Article/details/gtpvyoift.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.fehbvm.com/Article/details/gcqbsarfs.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.fehbvm.com/Article/details/gptzghris.sHtML

[S03] C：读入整数
来源：http://www.m.share.hesvh.cn/Article/details/ggjmdfzym.sHtML

int x; scanf("%d", &x);
来源：http://baike.hesvh.cn/Article/details/gjwouasir.sHtML

[S04] C：字符串复制
来源：http://read.share.fehbvm.com/Article/details/gllqfgxgf.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.hesvh.cn/Article/details/gqnwpyezs.sHtML

[S05] C：字符串长度
来源：http://wap.hesvh.cn/Article/details/ggufehoxs.sHtML

strlen(s)
来源：http://baike.fehbvm.com/Article/details/gpiajszxn.sHtML

[S06] C：字符串比较
来源：http://3g.fehbvm.com/Article/details/gzwytncpx.sHtML

strcmp(a, b) == 0
来源：http://mobile.fehbvm.com/Article/details/gooljpwhc.sHtML

[S07] C：数组遍历求和
来源：http://wap.fehbvm.com/Article/details/guzuhrful.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.zdbjq.cn/Article/details/ggmottmet.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.fehbvm.com/Article/details/gqnjntdyf.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.hesvh.cn/Article/details/grejlvukf.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.zdbjq.cn/Article/details/gchizkucn.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.hesvh.cn/Article/details/gzbcdbmoc.sHtML

[S10] C：指针与解引用
来源：http://3g.fehbvm.com/Article/details/gadknsqpz.sHtML

int *p = &a;  *p = 5;
来源：http://wap.fehbvm.com/Article/details/gtcegqeqb.sHtML

[S11] C：逐行读文件
来源：http://read.share.hesvh.cn/Article/details/ggmyieepl.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.hesvh.cn/Article/details/gvcsjbkum.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.hesvh.cn/Article/details/gtgoeotjd.sHtML

fclose(f);
来源：http://blog.fehbvm.com/Article/details/ghluukllx.sHtML

[S12] C：写文件
来源：http://mobile.zdbjq.cn/Article/details/gsxghrtmj.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.hesvh.cn/Article/details/gyswhjiha.sHtML

[S13] C：宏定义
来源：http://wap.hesvh.cn/Article/details/gyspznlwm.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.fehbvm.com/Article/details/gmcddiwbe.sHtML

[S14] C：枚举
来源：http://blog.fehbvm.com/Article/details/gjobubbyl.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.fehbvm.com/Article/details/gvzlexobw.sHtML

[S15] C：类型转换
来源：http://www.m.share.hesvh.cn/Article/details/gwyjfkrjm.sHtML

(double) a / b
来源：http://mobile.zdbjq.cn/Article/details/gyefxfehw.sHtML

[S16] C：位操作置位
来源：http://read.share.fehbvm.com/Article/details/gefcvubhx.sHtML

x |= (1 << 3);
来源：http://mobile.hesvh.cn/Article/details/gyexponso.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.fehbvm.com/Article/details/ggksgtcws.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.hesvh.cn/Article/details/gijhvvgua.sHtML

[S18] C：命令行参数
来源：http://blog.hesvh.cn/Article/details/gbweqrtdi.sHtML

int main(int argc, char **argv)
来源：http://www.blog.hesvh.cn/Article/details/gpzulsmdz.sHtML

[S19] C：快速排序
来源：http://www.share.fehbvm.com/Article/details/grghqptjw.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.fehbvm.com/Article/details/gvkhugxbz.sHtML

[S20] C：二分查找
来源：http://mobile.fehbvm.com/Article/details/gpwadylyf.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.hesvh.cn/Article/details/gohyzgvuv.sHtML

[S21] C：字符类别判断
来源：http://m.share.zdbjq.cn/Article/details/gttchqoik.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.fehbvm.com/Article/details/gwdvinyjc.sHtML

[S22] C：字符串转数字
来源：http://m.share.fehbvm.com/Article/details/grqulqddr.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.zdbjq.cn/Article/details/gtrlsjbzt.sHtML

[S23] C：随机数
来源：http://read.share.zdbjq.cn/Article/details/gxpezoaqn.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.hesvh.cn/Article/details/gieklhqrv.sHtML

[S24] C：获取本地时间
来源：http://www.blog.hesvh.cn/Article/details/gestdmrwa.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.fehbvm.com/Article/details/glvvrejdq.sHtML

[S25] C：内存拷贝
来源：http://www.share.zdbjq.cn/Article/details/gpvvsmyaj.sHtML

memcpy(dst, src, n);
来源：http://read.share.hesvh.cn/Article/details/gcxwbzisy.sHtML

[S26] C：内存清零
来源：http://wap.hesvh.cn/Article/details/gbjvxmuui.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.zdbjq.cn/Article/details/gessnadaw.sHtML

[S27] C：定义常量
来源：http://www.m.share.fehbvm.com/Article/details/gkxdhxgsr.sHtML

const double PI = 3.14159;
来源：http://blog.hesvh.cn/Article/details/gmqqecpyg.sHtML

[S28] C：静态变量
来源：http://www.blog.fehbvm.com/Article/details/gaboutjnz.sHtML

static int counter = 0;
来源：http://read.share.zdbjq.cn/Article/details/ghdogsdze.sHtML

[S29] C：变参函数
来源：http://www.m.share.hesvh.cn/Article/details/gjgmhpvdp.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.hesvh.cn/Article/details/gqwsduxmv.sHtML

[S30] C：头文件保护
来源：http://www.m.share.zdbjq.cn/Article/details/gjxsnrddx.sHtML

#ifndef X_H
来源：http://baike.zdbjq.cn/Article/details/gjbjviilc.sHtML

#define X_H
来源：http://m.share.fehbvm.com/Article/details/glocyaskz.sHtML

#endif
来源：http://mobile.zdbjq.cn/Article/details/glatfawwe.sHtML

[S31] C++：Hello World
来源：http://www.blog.fehbvm.com/Article/details/gthhutlxs.sHtML

#include <iostream>
来源：http://read.share.zdbjq.cn/Article/details/gtwjefjmi.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.zdbjq.cn/Article/details/gfwdnybtx.sHtML

[S32] C++：字符串
来源：http://wap.hesvh.cn/Article/details/gaoczfpir.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.zdbjq.cn/Article/details/gnsuxcali.sHtML

[S33] C++：vector 增删
来源：http://baike.hesvh.cn/Article/details/gdlvhxcxz.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.hesvh.cn/Article/details/gjrkgfbwe.sHtML

[S34] C++：遍历 vector
来源：http://www.share.hesvh.cn/Article/details/gymkipwdb.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.fehbvm.com/Article/details/gcutjmlmn.sHtML

[S35] C++：map
来源：http://blog.zdbjq.cn/Article/details/gsgflsnta.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.zdbjq.cn/Article/details/gnfaiejud.sHtML

[S36] C++：unordered_map
来源：http://wap.zdbjq.cn/Article/details/gxpkzkejs.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.hesvh.cn/Article/details/ggbdcequf.sHtML

[S37] C++：set
来源：http://m.share.fehbvm.com/Article/details/ghnoontxn.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.hesvh.cn/Article/details/glwqmzgqy.sHtML

[S38] C++：排序
来源：http://blog.fehbvm.com/Article/details/gaifhbepj.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.zdbjq.cn/Article/details/gzltgyuym.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.zdbjq.cn/Article/details/gucsddfgs.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.fehbvm.com/Article/details/guluwxwdc.sHtML

[S40] C++：查找元素
来源：http://wap.hesvh.cn/Article/details/gaybauvqy.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.hesvh.cn/Article/details/gkduyotxg.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.fehbvm.com/Article/details/glppmtrjw.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.hesvh.cn/Article/details/gfktxgrig.sHtML

[S42] C++：继承与虚函数
来源：http://3g.zdbjq.cn/Article/details/guvyecwyt.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.hesvh.cn/Article/details/gltvtpwqv.sHtML

[S43] C++：智能指针
来源：http://3g.fehbvm.com/Article/details/gldrnmzdc.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.fehbvm.com/Article/details/gbodwyerx.sHtML

[S44] C++：引用传参
来源：http://3g.fehbvm.com/Article/details/gonkjpbmd.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.hesvh.cn/Article/details/gfffkxexs.sHtML

[S45] C++：lambda
来源：http://m.share.fehbvm.com/Article/details/gzllqtloa.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.hesvh.cn/Article/details/gucifjriu.sHtML

[S46] C++：函数模板
来源：http://www.blog.fehbvm.com/Article/details/gmyoxcxqe.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.zdbjq.cn/Article/details/gkuhffaif.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.hesvh.cn/Article/details/gefrsfwhy.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.hesvh.cn/Article/details/gwxiqbbjq.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.fehbvm.com/Article/details/grhjblwwo.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.hesvh.cn/Article/details/gkgkbflrq.sHtML

while (std::getline(in, line)) { }
来源：http://wap.hesvh.cn/Article/details/ggiybwblm.sHtML

[S49] C++：写文件
来源：http://www.share.hesvh.cn/Article/details/gywmmkqiw.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.zdbjq.cn/Article/details/ghieonwqe.sHtML

[S50] C++：格式化数字
来源：http://3g.fehbvm.com/Article/details/gslijsgct.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.zdbjq.cn/Article/details/gofmmkgtm.sHtML

[S51] C++：显式类型转换
来源：http://baike.hesvh.cn/Article/details/gooocmrty.sHtML

static_cast<double>(a) / b
来源：http://mobile.hesvh.cn/Article/details/ghdybjqol.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.fehbvm.com/Article/details/gpugxrwlc.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.zdbjq.cn/Article/details/gwravudep.sHtML

[S53] C++：移动语义
来源：http://wap.hesvh.cn/Article/details/grtqubmbp.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.fehbvm.com/Article/details/gqrclhvwc.sHtML

[S54] C++：异常处理
来源：http://3g.hesvh.cn/Article/details/gkdzsngum.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.fehbvm.com/Article/details/gzzzqxnoy.sHtML

[S55] C++：结构化绑定
来源：http://m.share.fehbvm.com/Article/details/gzvvvlksq.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.fehbvm.com/Article/details/grojiurhl.sHtML

[S56] C++：optional
来源：http://blog.fehbvm.com/Article/details/gvdhskeof.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.hesvh.cn/Article/details/gnszfujat.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.hesvh.cn/Article/details/geqipgzme.sHtML

constexpr int N = 10;
来源：http://m.share.zdbjq.cn/Article/details/getxwhdkf.sHtML

[S58] C++：命名空间
来源：http://blog.fehbvm.com/Article/details/gkjdbmbuz.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.zdbjq.cn/Article/details/glpdiqpae.sHtML

[S59] C++：静态断言
来源：http://mobile.fehbvm.com/Article/details/geaxggpuz.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.hesvh.cn/Article/details/gtgilcehc.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.fehbvm.com/Article/details/gzshrashs.sHtML


<!-- 参考信息 -->