代发 wailian999

R. Bash 专题
来源：http://www.share.zdbjq.cn/Article/details/gygouqhof.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gvdywevag.sHtML

[R01] shebang 与严格模式
来源：http://blog.zdbjq.cn/Article/details/gjggmzftt.sHtML

#!/usr/bin/env bash
来源：http://blog.fehbvm.com/Article/details/gelbsesbs.sHtML

set -euo pipefail
来源：http://read.share.zdbjq.cn/Article/details/gbotdyish.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.hesvh.cn/Article/details/grjnuucqa.sHtML

name="Tom"; echo "$name"
来源：http://blog.fehbvm.com/Article/details/gnppekqjy.sHtML

[R03] 只读变量
来源：http://mobile.hesvh.cn/Article/details/gsstodsyq.sHtML

readonly PI=3.14
来源：http://blog.zdbjq.cn/Article/details/ggihfbvgz.sHtML

[R04] 位置参数
来源：http://read.share.fehbvm.com/Article/details/gnmtiiglo.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.zdbjq.cn/Article/details/gugacloat.sHtML

[R05] 参数默认值
来源：http://www.blog.hesvh.cn/Article/details/gxsraipwc.sHtML

name="${1:-default}"
来源：http://baike.fehbvm.com/Article/details/gxoesrtcs.sHtML

[R06] 判断命令是否存在
来源：http://3g.zdbjq.cn/Article/details/gmklopqfr.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.zdbjq.cn/Article/details/gjqzalddv.sHtML

[R07] if 判断文件
来源：http://www.share.zdbjq.cn/Article/details/gjnjthnki.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.hesvh.cn/Article/details/gphlyyyni.sHtML

[R08] 数值比较
来源：http://blog.fehbvm.com/Article/details/gcyobyzpy.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.zdbjq.cn/Article/details/gnkocklrp.sHtML

[R09] 字符串比较
来源：http://blog.hesvh.cn/Article/details/garqjbnyg.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.zdbjq.cn/Article/details/gjuuhohrl.sHtML

[R10] 正则匹配
来源：http://blog.hesvh.cn/Article/details/gtocufycn.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.fehbvm.com/Article/details/grrwttlwk.sHtML

[R11] case 多分支
来源：http://m.share.zdbjq.cn/Article/details/gfduqeemk.sHtML

case "$1" in
来源：http://baike.fehbvm.com/Article/details/gvdpvmpas.sHtML

start) echo "启动" ;;
来源：http://www.share.fehbvm.com/Article/details/gvgmjvjao.sHtML

stop)  echo "停止" ;;
来源：http://3g.zdbjq.cn/Article/details/gfcqracut.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.hesvh.cn/Article/details/gzbvzvudl.sHtML

esac
来源：http://wap.zdbjq.cn/Article/details/gsgwnzdit.sHtML

[R12] for 遍历文件
来源：http://wap.hesvh.cn/Article/details/gqhmmskqk.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.zdbjq.cn/Article/details/gaqavupfu.sHtML

[R13] for 计数循环
来源：http://m.share.hesvh.cn/Article/details/gxwudkctp.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.zdbjq.cn/Article/details/gowrniqoz.sHtML

[R14] C 风格 for
来源：http://3g.zdbjq.cn/Article/details/gormpkohk.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.hesvh.cn/Article/details/gxhebncgg.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.fehbvm.com/Article/details/gzfrthhtc.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.share.zdbjq.cn/Article/details/gafryvxhy.sHtML

[R16] until 等待条件
来源：http://www.share.zdbjq.cn/Article/details/ggtxizxqe.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.fehbvm.com/Article/details/goctblbgc.sHtML

[R17] 数组定义与取值
来源：http://baike.fehbvm.com/Article/details/gncagnhrx.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.hesvh.cn/Article/details/gbhhfogdf.sHtML

[R18] 遍历数组
来源：http://wap.hesvh.cn/Article/details/guxmwpxmv.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.m.share.zdbjq.cn/Article/details/gedezbsap.sHtML

[R19] 数组长度
来源：http://wap.zdbjq.cn/Article/details/ggepqqygr.sHtML

echo "${#arr[@]}"
来源：http://3g.fehbvm.com/Article/details/gpbmqcidg.sHtML

[R20] 关联数组（字典）
来源：http://baike.hesvh.cn/Article/details/grlokjmlj.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.zdbjq.cn/Article/details/grtahzyul.sHtML

[R21] 字符串长度
来源：http://www.blog.zdbjq.cn/Article/details/gscafoilb.sHtML

echo "${#s}"
来源：http://3g.fehbvm.com/Article/details/gvzgpfdyb.sHtML

[R22] 截取子串
来源：http://3g.fehbvm.com/Article/details/gaxgcncwy.sHtML

echo "${s:0:5}"
来源：http://baike.zdbjq.cn/Article/details/gwavnjoom.sHtML

[R23] 字符串替换
来源：http://read.share.zdbjq.cn/Article/details/goisokpay.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.fehbvm.com/Article/details/gcrsclnvn.sHtML

[R24] 大小写转换
来源：http://wap.hesvh.cn/Article/details/gnzustsso.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.fehbvm.com/Article/details/gchuybwwv.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.zdbjq.cn/Article/details/gdhqwayym.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.hesvh.cn/Article/details/glafhhuuv.sHtML

[R26] 命令替换
来源：http://blog.hesvh.cn/Article/details/gtwkfajjr.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.hesvh.cn/Article/details/gvlxkdxah.sHtML

[R27] 算术展开
来源：http://www.share.hesvh.cn/Article/details/gfenwviss.sHtML

echo $((1 + 2 * 3))
来源：http://baike.fehbvm.com/Article/details/gpwupkfzk.sHtML

[R28] 浮点运算
来源：http://3g.zdbjq.cn/Article/details/gnlsjsklo.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.zdbjq.cn/Article/details/gwqhqjxjx.sHtML

[R29] 定义函数
来源：http://mobile.fehbvm.com/Article/details/gfbklhelr.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.hesvh.cn/Article/details/gmvrbihjp.sHtML

[R30] 函数返回状态码
来源：http://www.blog.zdbjq.cn/Article/details/gokqocpzo.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.zdbjq.cn/Article/details/gpghjmnhc.sHtML

[R31] 局部变量
来源：http://3g.hesvh.cn/Article/details/gcnhfelgm.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.fehbvm.com/Article/details/ghjswmxxr.sHtML

[R32] 参数个数校验
来源：http://www.m.share.fehbvm.com/Article/details/gyexzpguo.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.fehbvm.com/Article/details/gdmouhxbd.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.hesvh.cn/Article/details/gfsaxwnhv.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.zdbjq.cn/Article/details/gglllyyyr.sHtML

[R34] 退出时清理
来源：http://mobile.zdbjq.cn/Article/details/gsqulwhls.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.hesvh.cn/Article/details/gcjwfucob.sHtML

[R35] 后台执行并等待
来源：http://3g.hesvh.cn/Article/details/grxxqzjto.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.hesvh.cn/Article/details/gqlmnbmvc.sHtML

[R36] 并发执行多个任务
来源：http://www.share.zdbjq.cn/Article/details/gfxadfxsy.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.hesvh.cn/Article/details/ghsrlhcej.sHtML

[R37] 把输出赋给变量
来源：http://baike.hesvh.cn/Article/details/gnpmvqklj.sHtML

files=$(ls -1)
来源：http://3g.fehbvm.com/Article/details/gmtlslpxo.sHtML

[R38] 管道串联
来源：http://blog.zdbjq.cn/Article/details/gsvkxzbtl.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.zdbjq.cn/Article/details/gxmtnhrlt.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.hesvh.cn/Article/details/garftmctm.sHtML

cmd > out.log 2>&1
来源：http://m.share.hesvh.cn/Article/details/gloshzpew.sHtML

[R40] 追加写日志
来源：http://baike.zdbjq.cn/Article/details/gfqetpfuz.sHtML

echo "log" >> out.log
来源：http://www.share.hesvh.cn/Article/details/guyqrxvqv.sHtML

[R41] 丢弃输出
来源：http://mobile.hesvh.cn/Article/details/gylqddqws.sHtML

cmd >/dev/null 2>&1
来源：http://www.blog.hesvh.cn/Article/details/gdeaquexo.sHtML

[R42] 输入重定向
来源：http://m.share.fehbvm.com/Article/details/gqhbqjeyh.sHtML

wc -l < a.txt
来源：http://mobile.hesvh.cn/Article/details/gxfgnyhsn.sHtML

[R43] 按名字查找文件
来源：http://m.share.fehbvm.com/Article/details/gazuxyqby.sHtML

find . -name "*.log" -type f
来源：http://3g.fehbvm.com/Article/details/gdsvkbvvo.sHtML

[R44] 按修改时间查找
来源：http://read.share.fehbvm.com/Article/details/gyewdoxxh.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.zdbjq.cn/Article/details/gbcortlsy.sHtML

[R45] 批量删除
来源：http://www.share.zdbjq.cn/Article/details/gppbkwstl.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.hesvh.cn/Article/details/gfzhxvqhe.sHtML

[R46] 递归替换文件内容
来源：http://read.share.hesvh.cn/Article/details/guosoivja.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.hesvh.cn/Article/details/gugntcgdz.sHtML

[R47] sed 单行替换
来源：http://www.blog.fehbvm.com/Article/details/gavemsppq.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.hesvh.cn/Article/details/gipjodtsn.sHtML

[R48] awk 取指定列
来源：http://wap.zdbjq.cn/Article/details/gddhcthjx.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.hesvh.cn/Article/details/gtktttpww.sHtML

[R49] awk 带条件
来源：http://mobile.zdbjq.cn/Article/details/gzgpmuasy.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.hesvh.cn/Article/details/gzbfvojee.sHtML

[R50] awk 求和
来源：http://blog.hesvh.cn/Article/details/goxapiqop.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.hesvh.cn/Article/details/gexbipjdd.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.zdbjq.cn/Article/details/gfzzampvb.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.zdbjq.cn/Article/details/gxfeqgsrq.sHtML

[R52] 统计行数
来源：http://m.share.zdbjq.cn/Article/details/gzrnlmsfk.sHtML

wc -l a.txt
来源：http://wap.zdbjq.cn/Article/details/ghbtwaerm.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.zdbjq.cn/Article/details/ginsztxni.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.fehbvm.com/Article/details/gcbfctydx.sHtML

[R54] 比较两个文件
来源：http://mobile.zdbjq.cn/Article/details/gzyvajbyq.sHtML

diff a.txt b.txt
来源：http://3g.zdbjq.cn/Article/details/gxuaeyszf.sHtML

[R55] 压缩与解压
来源：http://baike.zdbjq.cn/Article/details/gkrwdvaxl.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.hesvh.cn/Article/details/gcjpphjjm.sHtML

[R56] 远程拷贝
来源：http://m.share.fehbvm.com/Article/details/gdyigtltc.sHtML

scp file user@host:/path/
来源：http://wap.hesvh.cn/Article/details/ghwrrowzz.sHtML

[R57] 远程执行命令
来源：http://wap.hesvh.cn/Article/details/gjtnesycu.sHtML

ssh user@host 'uptime'
来源：http://mobile.fehbvm.com/Article/details/gpcuuvdfo.sHtML

[R58] 下载文件
来源：http://read.share.zdbjq.cn/Article/details/gosnvwijt.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.fehbvm.com/Article/details/ghnktlodn.sHtML

[R59] 发 POST JSON
来源：http://www.share.fehbvm.com/Article/details/gwcafgxcj.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.fehbvm.com/Article/details/gkrjiojbh.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.zdbjq.cn/Article/details/gedsrwrim.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.hesvh.cn/Article/details/gbsekouak.sHtML

[R61] 磁盘占用
来源：http://mobile.fehbvm.com/Article/details/gdbjpncgy.sHtML

df -h;  du -sh *
来源：http://read.share.zdbjq.cn/Article/details/gnwelbray.sHtML

[R62] 找最占空间的文件
来源：http://baike.hesvh.cn/Article/details/gmxjwicnb.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.zdbjq.cn/Article/details/gopnfjvvq.sHtML

[R63] 内存与进程
来源：http://m.share.fehbvm.com/Article/details/gxtyemolz.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.zdbjq.cn/Article/details/giivhkqwl.sHtML

[R64] 结束进程
来源：http://blog.zdbjq.cn/Article/details/gwrptfccf.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.zdbjq.cn/Article/details/grhlwmgug.sHtML

[R65] 查看端口占用
来源：http://mobile.zdbjq.cn/Article/details/gszowfjtt.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.zdbjq.cn/Article/details/ggsnbyygl.sHtML

[R66] 定时任务
来源：http://blog.fehbvm.com/Article/details/gaklhufra.sHtML

crontab -e;  crontab -l
来源：http://3g.fehbvm.com/Article/details/gtafevawr.sHtML

[R67] 生成随机十六进制串
来源：http://wap.hesvh.cn/Article/details/gmxyptpdg.sHtML

openssl rand -hex 16
来源：http://www.share.hesvh.cn/Article/details/gqkldotln.sHtML

[R68] 计算文件校验值
来源：http://wap.fehbvm.com/Article/details/gewyuwnyo.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.zdbjq.cn/Article/details/gemahjkye.sHtML

[R69] 生成随机密码
来源：http://mobile.zdbjq.cn/Article/details/guwedxtyy.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.fehbvm.com/Article/details/gxojioxnq.sHtML

[R70] 时间戳与互转
来源：http://m.share.fehbvm.com/Article/details/gdrztyvkm.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.hesvh.cn/Article/details/gnfkbmlkl.sHtML

[R71] 日期格式化
来源：http://mobile.hesvh.cn/Article/details/gdcoluodu.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.zdbjq.cn/Article/details/gkcctapdv.sHtML

[R72] 等待端口就绪
来源：http://3g.fehbvm.com/Article/details/grfxlyupz.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.zdbjq.cn/Article/details/gkmnvcmec.sHtML

[R73] 分割大日志
来源：http://mobile.zdbjq.cn/Article/details/ghsyirgdg.sHtML

split -l 1000 big.log part_
来源：http://wap.zdbjq.cn/Article/details/giwkmhwee.sHtML

[R74] 批量重命名
来源：http://www.share.hesvh.cn/Article/details/gzbyzxrnx.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.hesvh.cn/Article/details/gjtachyvb.sHtML

[R75] 导出环境变量
来源：http://www.share.hesvh.cn/Article/details/gswktyrwk.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.hesvh.cn/Article/details/gcbsgirmo.sHtML

[R76] 使用临时文件
来源：http://www.m.share.zdbjq.cn/Article/details/ggnnbhpko.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.hesvh.cn/Article/details/grfyqmtug.sHtML

[R77] 读取用户输入
来源：http://www.share.hesvh.cn/Article/details/gvagutmyr.sHtML

read -rp "请输入: " ans
来源：http://m.share.hesvh.cn/Article/details/gpirfdzxl.sHtML

[R78] 交互式菜单
来源：http://wap.zdbjq.cn/Article/details/gxhawdqkl.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.zdbjq.cn/Article/details/gyeyntmvp.sHtML

[R79] 解析命令行选项
来源：http://blog.hesvh.cn/Article/details/gwzpcoqce.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.hesvh.cn/Article/details/gzjxzudxm.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.fehbvm.com/Article/details/glnmrjibg.sHtML

time ./run.sh
来源：http://blog.hesvh.cn/Article/details/gxcaqbdpp.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gnkaelnjp.sHtML

S. C / C++ 专题
来源：http://read.share.fehbvm.com/Article/details/gyxbbliqk.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/getgehcjs.sHtML

[S01] C：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gvitusrru.sHtML

#include <stdio.h>
来源：http://m.share.zdbjq.cn/Article/details/gsjiarcpx.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.fehbvm.com/Article/details/ggkrcjfic.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.fehbvm.com/Article/details/gynegjrvl.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.hesvh.cn/Article/details/gwdgnqlab.sHtML

[S03] C：读入整数
来源：http://wap.hesvh.cn/Article/details/giznlcijz.sHtML

int x; scanf("%d", &x);
来源：http://mobile.zdbjq.cn/Article/details/gmatztaqr.sHtML

[S04] C：字符串复制
来源：http://www.share.zdbjq.cn/Article/details/gkvzobray.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.zdbjq.cn/Article/details/gjozlenwb.sHtML

[S05] C：字符串长度
来源：http://blog.zdbjq.cn/Article/details/gmycaowjj.sHtML

strlen(s)
来源：http://baike.hesvh.cn/Article/details/gdivzrlax.sHtML

[S06] C：字符串比较
来源：http://blog.hesvh.cn/Article/details/gtsdnzwlf.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.hesvh.cn/Article/details/gbsgprknt.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.hesvh.cn/Article/details/gkxbmhwcq.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.hesvh.cn/Article/details/ggalwniar.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.hesvh.cn/Article/details/gzlbquvbf.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.zdbjq.cn/Article/details/gzlvaippl.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.fehbvm.com/Article/details/gtxaebutt.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.fehbvm.com/Article/details/gullbloub.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.fehbvm.com/Article/details/godlvgsqq.sHtML

int *p = &a;  *p = 5;
来源：http://baike.hesvh.cn/Article/details/gnrgnnnxf.sHtML

[S11] C：逐行读文件
来源：http://blog.fehbvm.com/Article/details/gdawtppue.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.zdbjq.cn/Article/details/ggnyfxbnr.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.zdbjq.cn/Article/details/ghlakmcsp.sHtML

fclose(f);
来源：http://www.share.fehbvm.com/Article/details/gzeiiduri.sHtML

[S12] C：写文件
来源：http://read.share.hesvh.cn/Article/details/gnzcqwadl.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.fehbvm.com/Article/details/gjhposbsh.sHtML

[S13] C：宏定义
来源：http://3g.zdbjq.cn/Article/details/gfddexvkg.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.zdbjq.cn/Article/details/gxchwuvqq.sHtML

[S14] C：枚举
来源：http://read.share.hesvh.cn/Article/details/ggahiylhw.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.hesvh.cn/Article/details/gwnamhfsn.sHtML

[S15] C：类型转换
来源：http://3g.zdbjq.cn/Article/details/glrviiyju.sHtML

(double) a / b
来源：http://www.blog.fehbvm.com/Article/details/gkvknnzst.sHtML

[S16] C：位操作置位
来源：http://3g.zdbjq.cn/Article/details/gjguzllwr.sHtML

x |= (1 << 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gxlxtklkp.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.zdbjq.cn/Article/details/gsbcslada.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.hesvh.cn/Article/details/gjishmhzw.sHtML

[S18] C：命令行参数
来源：http://wap.hesvh.cn/Article/details/gbxsdpdkq.sHtML

int main(int argc, char **argv)
来源：http://www.share.fehbvm.com/Article/details/guatqbnsa.sHtML

[S19] C：快速排序
来源：http://wap.zdbjq.cn/Article/details/gljvxsjfh.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.hesvh.cn/Article/details/guvligkmz.sHtML

[S20] C：二分查找
来源：http://www.blog.zdbjq.cn/Article/details/ghudumsah.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.hesvh.cn/Article/details/giqxvtceh.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.hesvh.cn/Article/details/gparmfbwe.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.hesvh.cn/Article/details/ggmmcenwh.sHtML

[S22] C：字符串转数字
来源：http://3g.zdbjq.cn/Article/details/gqnirwzid.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.fehbvm.com/Article/details/gczkipcpq.sHtML

[S23] C：随机数
来源：http://www.m.share.hesvh.cn/Article/details/gvtkjqzly.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.hesvh.cn/Article/details/gwobozcmm.sHtML

[S24] C：获取本地时间
来源：http://www.blog.fehbvm.com/Article/details/gixneiugl.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.hesvh.cn/Article/details/gbijtyurk.sHtML

[S25] C：内存拷贝
来源：http://m.share.hesvh.cn/Article/details/gxmczcnst.sHtML

memcpy(dst, src, n);
来源：http://www.share.hesvh.cn/Article/details/gtzgtauhc.sHtML

[S26] C：内存清零
来源：http://www.m.share.fehbvm.com/Article/details/gjjmorqwm.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.zdbjq.cn/Article/details/gceucxuri.sHtML

[S27] C：定义常量
来源：http://3g.fehbvm.com/Article/details/gsgrtrwwo.sHtML

const double PI = 3.14159;
来源：http://mobile.fehbvm.com/Article/details/gptvgwdnl.sHtML

[S28] C：静态变量
来源：http://mobile.fehbvm.com/Article/details/gjeuknlhe.sHtML

static int counter = 0;
来源：http://blog.zdbjq.cn/Article/details/geascxsbh.sHtML

[S29] C：变参函数
来源：http://3g.zdbjq.cn/Article/details/gjllhgaos.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.fehbvm.com/Article/details/gmaznkhuq.sHtML

[S30] C：头文件保护
来源：http://www.share.hesvh.cn/Article/details/gyringrmd.sHtML

#ifndef X_H
来源：http://3g.fehbvm.com/Article/details/ggsoamsir.sHtML

#define X_H
来源：http://wap.zdbjq.cn/Article/details/gyvvmodae.sHtML

#endif
来源：http://www.blog.hesvh.cn/Article/details/gyuqubshp.sHtML

[S31] C++：Hello World
来源：http://wap.hesvh.cn/Article/details/gqbjulvog.sHtML

#include <iostream>
来源：http://m.share.hesvh.cn/Article/details/gzuwznsxz.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.hesvh.cn/Article/details/gyppwlmyj.sHtML

[S32] C++：字符串
来源：http://wap.fehbvm.com/Article/details/gszoxlzpn.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.fehbvm.com/Article/details/grqowpybh.sHtML

[S33] C++：vector 增删
来源：http://wap.hesvh.cn/Article/details/guosqsiwc.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.zdbjq.cn/Article/details/ghvmtftoc.sHtML

[S34] C++：遍历 vector
来源：http://www.share.fehbvm.com/Article/details/ghhllwhzp.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.zdbjq.cn/Article/details/grjinevjv.sHtML

[S35] C++：map
来源：http://wap.fehbvm.com/Article/details/glbuguldt.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/gfuhkshhh.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.zdbjq.cn/Article/details/gjdzdkxqn.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/ghxvzfpdx.sHtML

[S37] C++：set
来源：http://mobile.fehbvm.com/Article/details/gkxylwpfj.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.fehbvm.com/Article/details/gwonlhqjs.sHtML

[S38] C++：排序
来源：http://www.share.hesvh.cn/Article/details/gdnipuunx.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.fehbvm.com/Article/details/gaiozwdii.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.fehbvm.com/Article/details/gdpkbydot.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.fehbvm.com/Article/details/gldubduov.sHtML

[S40] C++：查找元素
来源：http://mobile.hesvh.cn/Article/details/gnxhtajtm.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.zdbjq.cn/Article/details/gdxkbhqqa.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.hesvh.cn/Article/details/giklldybj.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.fehbvm.com/Article/details/gxfhsucfs.sHtML

[S42] C++：继承与虚函数
来源：http://baike.zdbjq.cn/Article/details/gueisrxin.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.zdbjq.cn/Article/details/gfqgpotpm.sHtML

[S43] C++：智能指针
来源：http://www.blog.zdbjq.cn/Article/details/glidanygm.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.hesvh.cn/Article/details/gkpglyxnh.sHtML

[S44] C++：引用传参
来源：http://m.share.zdbjq.cn/Article/details/gzcerejme.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.fehbvm.com/Article/details/gojraextn.sHtML

[S45] C++：lambda
来源：http://www.share.zdbjq.cn/Article/details/glinxmxhi.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.zdbjq.cn/Article/details/gysnwfwcn.sHtML

[S46] C++：函数模板
来源：http://www.share.fehbvm.com/Article/details/ggootwxpr.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.zdbjq.cn/Article/details/gmjlkjztz.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.fehbvm.com/Article/details/gvihfoxfk.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.hesvh.cn/Article/details/gtmhmwtzt.sHtML

[S48] C++：逐行读文件
来源：http://read.share.zdbjq.cn/Article/details/gqugsmzzb.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.fehbvm.com/Article/details/gvtcmikxo.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.hesvh.cn/Article/details/gnjeezldz.sHtML

[S49] C++：写文件
来源：http://wap.zdbjq.cn/Article/details/gtfmpvynm.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.hesvh.cn/Article/details/gqwqokkhh.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.hesvh.cn/Article/details/gkqxaaecm.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.zdbjq.cn/Article/details/grscbxvlm.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.fehbvm.com/Article/details/gpckkrvge.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.zdbjq.cn/Article/details/gogjxctsv.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.hesvh.cn/Article/details/gfgrewxwd.sHtML

int size() const noexcept { return n_; }
来源：http://wap.zdbjq.cn/Article/details/guzpvkved.sHtML

[S53] C++：移动语义
来源：http://www.m.share.fehbvm.com/Article/details/grsymopmc.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.hesvh.cn/Article/details/ghamwizsq.sHtML

[S54] C++：异常处理
来源：http://m.share.fehbvm.com/Article/details/gqzufnwra.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.hesvh.cn/Article/details/gzbratlgr.sHtML

[S55] C++：结构化绑定
来源：http://baike.zdbjq.cn/Article/details/gpvjmorog.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.fehbvm.com/Article/details/gkuvdaujy.sHtML

[S56] C++：optional
来源：http://www.blog.hesvh.cn/Article/details/gpozvdsrw.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.fehbvm.com/Article/details/gmgracdjl.sHtML

[S57] C++：编译期常量
来源：http://wap.zdbjq.cn/Article/details/gaqiwvujg.sHtML

constexpr int N = 10;
来源：http://wap.hesvh.cn/Article/details/gkihymsjq.sHtML

[S58] C++：命名空间
来源：http://blog.hesvh.cn/Article/details/gypbqkgmd.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.fehbvm.com/Article/details/gtqkqybbz.sHtML

[S59] C++：静态断言
来源：http://mobile.zdbjq.cn/Article/details/gtvojwfbt.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.hesvh.cn/Article/details/giudnarys.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.zdbjq.cn/Article/details/gvriytrmc.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.fehbvm.com/Article/details/ganeyctum.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gydzcmxpb.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.zdbjq.cn/Article/details/gcvmovgfd.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gqpecyuvw.sHtML


<!-- 参考信息 -->