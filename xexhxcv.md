代发 wailian999

set -euo pipefail
来源：http://mobile.fanxiaobao.xyz/Article/details/gridoeuve.sHtML

[R02] 变量赋值与使用
来源：http://wap.fanxiaobao.xyz/Article/details/gtbrkdgvn.sHtML

name="Tom"; echo "$name"
来源：http://mobile.fanxiaobao.xyz/Article/details/ghbxdvste.sHtML

[R03] 只读变量
来源：http://wap.fanxiaobao.xyz/Article/details/gklssjhsp.sHtML

readonly PI=3.14
来源：http://www.share.fanxiaobao.xyz/Article/details/grqrsgzlt.sHtML

[R04] 位置参数
来源：http://mobile.fanxiaobao.xyz/Article/details/gfvvwfcdb.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.fanxiaobao.xyz/Article/details/gfllytubc.sHtML

[R05] 参数默认值
来源：http://m.share.fanxiaobao.xyz/Article/details/ggnokvkmi.sHtML

name="${1:-default}"
来源：http://baike.fanxiaobao.xyz/Article/details/glhhkiipn.sHtML

[R06] 判断命令是否存在
来源：http://www.share.fanxiaobao.xyz/Article/details/gdenlsozt.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gsyufyumr.sHtML

[R07] if 判断文件
来源：http://blog.fanxiaobao.xyz/Article/details/gqafshxvp.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.fanxiaobao.xyz/Article/details/gwiiavpvu.sHtML

[R08] 数值比较
来源：http://wap.fanxiaobao.xyz/Article/details/gpkbgzacg.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.fanxiaobao.xyz/Article/details/gjvnanuku.sHtML

[R09] 字符串比较
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpccwcpgv.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://3g.fanxiaobao.xyz/Article/details/gnrpqkcgl.sHtML

[R10] 正则匹配
来源：http://wap.fanxiaobao.xyz/Article/details/gzacssrcj.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.fanxiaobao.xyz/Article/details/gwlnknqnf.sHtML

[R11] case 多分支
来源：http://3g.fanxiaobao.xyz/Article/details/gkttxfkeh.sHtML

case "$1" in
来源：http://wap.fanxiaobao.xyz/Article/details/gbdostbqx.sHtML

start) echo "启动" ;;
来源：http://read.share.fanxiaobao.xyz/Article/details/gkmgicwiw.sHtML

stop)  echo "停止" ;;
来源：http://www.share.fanxiaobao.xyz/Article/details/gkpjkhnas.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.fanxiaobao.xyz/Article/details/grnpxince.sHtML

esac
来源：http://blog.fanxiaobao.xyz/Article/details/gluxyyahe.sHtML

[R12] for 遍历文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gympohokl.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gecolcnql.sHtML

[R13] for 计数循环
来源：http://www.share.fanxiaobao.xyz/Article/details/gxessbrnk.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.fanxiaobao.xyz/Article/details/gftqspngz.sHtML

[R14] C 风格 for
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gajaxyhly.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gisdbextn.sHtML

[R15] while 逐行读文件
来源：http://wap.fanxiaobao.xyz/Article/details/geijxmzih.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gwffreqni.sHtML

[R16] until 等待条件
来源：http://mobile.fanxiaobao.xyz/Article/details/gmyenmnna.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.fanxiaobao.xyz/Article/details/gslrvnlli.sHtML

[R17] 数组定义与取值
来源：http://www.share.fanxiaobao.xyz/Article/details/gnroyeyhr.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://3g.fanxiaobao.xyz/Article/details/gohrhtgce.sHtML

[R18] 遍历数组
来源：http://3g.fanxiaobao.xyz/Article/details/gurzrsltk.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/ggpnkjicc.sHtML

[R19] 数组长度
来源：http://mobile.fanxiaobao.xyz/Article/details/gckbpgtbv.sHtML

echo "${#arr[@]}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gpfzjfwfs.sHtML

[R20] 关联数组（字典）
来源：http://baike.fanxiaobao.xyz/Article/details/gsgrsazhs.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gkdpdnime.sHtML

[R21] 字符串长度
来源：http://blog.fanxiaobao.xyz/Article/details/gisqkjiqv.sHtML

echo "${#s}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gaunpvveq.sHtML

[R22] 截取子串
来源：http://blog.fanxiaobao.xyz/Article/details/gnzkmlovq.sHtML

echo "${s:0:5}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gwoiirqgq.sHtML

[R23] 字符串替换
来源：http://blog.fanxiaobao.xyz/Article/details/gwfsrgyop.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.fanxiaobao.xyz/Article/details/geibtamfz.sHtML

[R24] 大小写转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/grokujjjb.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.fanxiaobao.xyz/Article/details/gtvujjhlr.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.fanxiaobao.xyz/Article/details/gijozewfn.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gxqelpnvn.sHtML

[R26] 命令替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gcsbnepaa.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.fanxiaobao.xyz/Article/details/gmqgiisyp.sHtML

[R27] 算术展开
来源：http://read.share.fanxiaobao.xyz/Article/details/gcpptsdkp.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gimbnrxmt.sHtML

[R28] 浮点运算
来源：http://baike.fanxiaobao.xyz/Article/details/ghkvqewca.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsigtdeoq.sHtML

[R29] 定义函数
来源：http://3g.fanxiaobao.xyz/Article/details/gxmemesnh.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.fanxiaobao.xyz/Article/details/gwuhhllie.sHtML

[R30] 函数返回状态码
来源：http://www.share.fanxiaobao.xyz/Article/details/gebweisia.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.fanxiaobao.xyz/Article/details/gbaivaiyx.sHtML

[R31] 局部变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyrkpngey.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gdmxiqpox.sHtML

[R32] 参数个数校验
来源：http://mobile.fanxiaobao.xyz/Article/details/gwowwiyci.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gdxbvwvxr.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gedatzgei.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.fanxiaobao.xyz/Article/details/gbobfxnbs.sHtML

[R34] 退出时清理
来源：http://www.blog.fanxiaobao.xyz/Article/details/gatoonmgm.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fanxiaobao.xyz/Article/details/gyakfjpyb.sHtML

[R35] 后台执行并等待
来源：http://3g.fanxiaobao.xyz/Article/details/gswtcyrxm.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.fanxiaobao.xyz/Article/details/gslsvfbqn.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfgwbiqhi.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.fanxiaobao.xyz/Article/details/gsgdyvgkr.sHtML

[R37] 把输出赋给变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gwmlkgsbp.sHtML

files=$(ls -1)
来源：http://blog.fanxiaobao.xyz/Article/details/gdjxdagff.sHtML

[R38] 管道串联
来源：http://read.share.fanxiaobao.xyz/Article/details/gdugjxnvu.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.fanxiaobao.xyz/Article/details/ghlufkbpi.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.fanxiaobao.xyz/Article/details/gmrsnersi.sHtML

cmd > out.log 2>&1
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfnpiotix.sHtML

[R40] 追加写日志
来源：http://read.share.fanxiaobao.xyz/Article/details/glikcdnxc.sHtML

echo "log" >> out.log
来源：http://wap.fanxiaobao.xyz/Article/details/gexrjseml.sHtML

[R41] 丢弃输出
来源：http://blog.fanxiaobao.xyz/Article/details/gdlyxksax.sHtML

cmd >/dev/null 2>&1
来源：http://blog.fanxiaobao.xyz/Article/details/grbexvqex.sHtML

[R42] 输入重定向
来源：http://baike.fanxiaobao.xyz/Article/details/gpnufpgyg.sHtML

wc -l < a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gxlyupmdv.sHtML

[R43] 按名字查找文件
来源：http://m.share.fanxiaobao.xyz/Article/details/glczcqksd.sHtML

find . -name "*.log" -type f
来源：http://wap.fanxiaobao.xyz/Article/details/gqihyjwgz.sHtML

[R44] 按修改时间查找
来源：http://read.share.fanxiaobao.xyz/Article/details/gbcplmvon.sHtML

find . -mtime -7 -type f
来源：http://blog.fanxiaobao.xyz/Article/details/gpxnbcosw.sHtML

[R45] 批量删除
来源：http://wap.fanxiaobao.xyz/Article/details/gypqtmigi.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.fanxiaobao.xyz/Article/details/gxezgquvw.sHtML

[R46] 递归替换文件内容
来源：http://m.share.fanxiaobao.xyz/Article/details/gxvoxkmcs.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.fanxiaobao.xyz/Article/details/gmyeqblpa.sHtML

[R47] sed 单行替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gfgrfbwbl.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gobgxalaj.sHtML

[R48] awk 取指定列
来源：http://wap.fanxiaobao.xyz/Article/details/gbusmwlwr.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gbfidxwan.sHtML

[R49] awk 带条件
来源：http://m.share.fanxiaobao.xyz/Article/details/grzdegmxm.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.fanxiaobao.xyz/Article/details/gtavemylu.sHtML

[R50] awk 求和
来源：http://read.share.fanxiaobao.xyz/Article/details/gfojjdvjp.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gzpbnnngl.sHtML

[R51] 排序去重取前几
来源：http://www.blog.fanxiaobao.xyz/Article/details/gahodctar.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.fanxiaobao.xyz/Article/details/gxhzvzlub.sHtML

[R52] 统计行数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsivcmovh.sHtML

wc -l a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gkdojrqvu.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.fanxiaobao.xyz/Article/details/ggictmoku.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.fanxiaobao.xyz/Article/details/gwvktkfwc.sHtML

[R54] 比较两个文件
来源：http://blog.fanxiaobao.xyz/Article/details/ghpuwzctv.sHtML

diff a.txt b.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gneotzmga.sHtML

[R55] 压缩与解压
来源：http://m.share.fanxiaobao.xyz/Article/details/gdhjdeefp.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.fanxiaobao.xyz/Article/details/gijnzexyn.sHtML

[R56] 远程拷贝
来源：http://baike.fanxiaobao.xyz/Article/details/gtpbxuyld.sHtML

scp file user@host:/path/
来源：http://www.share.fanxiaobao.xyz/Article/details/geedolubj.sHtML

[R57] 远程执行命令
来源：http://mobile.fanxiaobao.xyz/Article/details/gbexrcbyt.sHtML

ssh user@host 'uptime'
来源：http://read.share.fanxiaobao.xyz/Article/details/gwqdcaaby.sHtML

[R58] 下载文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gmlidepdz.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.fanxiaobao.xyz/Article/details/gbvnelijd.sHtML

[R59] 发 POST JSON
来源：http://blog.fanxiaobao.xyz/Article/details/gynbnhyqx.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.fanxiaobao.xyz/Article/details/gtmgompxe.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.fanxiaobao.xyz/Article/details/gcoiatvnm.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.fanxiaobao.xyz/Article/details/ghzfzeidi.sHtML

[R61] 磁盘占用
来源：http://read.share.fanxiaobao.xyz/Article/details/glgpogvmy.sHtML

df -h;  du -sh *
来源：http://baike.fanxiaobao.xyz/Article/details/gehhiyljz.sHtML

[R62] 找最占空间的文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gwuehywqv.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.fanxiaobao.xyz/Article/details/gacumhnhz.sHtML

[R63] 内存与进程
来源：http://wap.fanxiaobao.xyz/Article/details/gcmdzjnls.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdkzmcacm.sHtML

[R64] 结束进程
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geopwbose.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.fanxiaobao.xyz/Article/details/gkpyqkzjx.sHtML

[R65] 查看端口占用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwpnfwhku.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gawuwamie.sHtML

[R66] 定时任务
来源：http://www.blog.fanxiaobao.xyz/Article/details/guopzwjvn.sHtML

crontab -e;  crontab -l
来源：http://wap.fanxiaobao.xyz/Article/details/grkglzsew.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gukzrfvpq.sHtML

openssl rand -hex 16
来源：http://www.share.fanxiaobao.xyz/Article/details/gaaganlnt.sHtML

[R68] 计算文件校验值
来源：http://wap.fanxiaobao.xyz/Article/details/gwwqkmhjq.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghzevjtuw.sHtML

[R69] 生成随机密码
来源：http://baike.fanxiaobao.xyz/Article/details/ggapyzhvt.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.fanxiaobao.xyz/Article/details/gijotzdhr.sHtML

[R70] 时间戳与互转
来源：http://3g.fanxiaobao.xyz/Article/details/gvsxntkoe.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpqjzeqrx.sHtML

[R71] 日期格式化
来源：http://wap.fanxiaobao.xyz/Article/details/gokofzqho.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gezgpajuf.sHtML

[R72] 等待端口就绪
来源：http://read.share.fanxiaobao.xyz/Article/details/gbohccuxd.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.fanxiaobao.xyz/Article/details/gqsmlaycs.sHtML

[R73] 分割大日志
来源：http://wap.fanxiaobao.xyz/Article/details/gjgjqcniq.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdnnyawzr.sHtML

[R74] 批量重命名
来源：http://www.share.fanxiaobao.xyz/Article/details/gpsvchzco.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/ghqnhbezs.sHtML

[R75] 导出环境变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghtythags.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.fanxiaobao.xyz/Article/details/gvogcmckq.sHtML

[R76] 使用临时文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpipbgliq.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtlckziqi.sHtML

[R77] 读取用户输入
来源：http://blog.fanxiaobao.xyz/Article/details/gmfvagtrh.sHtML

read -rp "请输入: " ans
来源：http://mobile.fanxiaobao.xyz/Article/details/gjekzyooa.sHtML

[R78] 交互式菜单
来源：http://mobile.fanxiaobao.xyz/Article/details/gfmpyeowy.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gronriiby.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwgnpofva.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvecgpqwh.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.fanxiaobao.xyz/Article/details/gssxsknec.sHtML

time ./run.sh
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkowrhfst.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gzejdamnh.sHtML

S. C / C++ 专题
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzwlhwweg.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gqcjequzx.sHtML

[S01] C：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gsurbgujt.sHtML

#include <stdio.h>
来源：http://read.share.fanxiaobao.xyz/Article/details/gnggpyjnj.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.fanxiaobao.xyz/Article/details/gpyknvvrg.sHtML

[S02] C：变量与格式化输出
来源：http://3g.fanxiaobao.xyz/Article/details/gizqmgpjq.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.fanxiaobao.xyz/Article/details/gqudskmzq.sHtML

[S03] C：读入整数
来源：http://mobile.fanxiaobao.xyz/Article/details/gzbltvhyh.sHtML

int x; scanf("%d", &x);
来源：http://mobile.fanxiaobao.xyz/Article/details/gwiyrllvm.sHtML

[S04] C：字符串复制
来源：http://wap.fanxiaobao.xyz/Article/details/gotyyyobg.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtutrynqe.sHtML

[S05] C：字符串长度
来源：http://read.share.fanxiaobao.xyz/Article/details/gmflfpdso.sHtML

strlen(s)
来源：http://baike.fanxiaobao.xyz/Article/details/gugqdhqaw.sHtML

[S06] C：字符串比较
来源：http://www.share.fanxiaobao.xyz/Article/details/gfexpslgp.sHtML

strcmp(a, b) == 0
来源：http://www.share.fanxiaobao.xyz/Article/details/gtqqxzvvi.sHtML

[S07] C：数组遍历求和
来源：http://m.share.fanxiaobao.xyz/Article/details/gmjubzmcy.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.fanxiaobao.xyz/Article/details/gvyakfkfu.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjktxnfpx.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.fanxiaobao.xyz/Article/details/gjhwribgz.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.fanxiaobao.xyz/Article/details/gbdauoanq.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.fanxiaobao.xyz/Article/details/gagpanxrh.sHtML

[S10] C：指针与解引用
来源：http://baike.fanxiaobao.xyz/Article/details/gepyqmjlv.sHtML

int *p = &a;  *p = 5;
来源：http://baike.fanxiaobao.xyz/Article/details/gjykpvkaj.sHtML

[S11] C：逐行读文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gtsiwkhhb.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.fanxiaobao.xyz/Article/details/gumxjthgp.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.fanxiaobao.xyz/Article/details/guitmsvhc.sHtML

fclose(f);
来源：http://www.share.fanxiaobao.xyz/Article/details/gdkckgsds.sHtML

[S12] C：写文件
来源：http://wap.fanxiaobao.xyz/Article/details/gfmtgpfxv.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.fanxiaobao.xyz/Article/details/gymkosxfe.sHtML

[S13] C：宏定义
来源：http://3g.fanxiaobao.xyz/Article/details/gefpyzaer.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.fanxiaobao.xyz/Article/details/gpftjqjgi.sHtML

[S14] C：枚举
来源：http://3g.fanxiaobao.xyz/Article/details/gghrqtkbx.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.fanxiaobao.xyz/Article/details/gcaxmauxp.sHtML

[S15] C：类型转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glhgjyolv.sHtML

(double) a / b
来源：http://mobile.fanxiaobao.xyz/Article/details/garbyzmdn.sHtML

[S16] C：位操作置位
来源：http://read.share.fanxiaobao.xyz/Article/details/gdazsabtb.sHtML

x |= (1 << 3);
来源：http://baike.fanxiaobao.xyz/Article/details/gesrjwzvh.sHtML

[S17] C：安全拼接字符串
来源：http://blog.fanxiaobao.xyz/Article/details/gyoludjcy.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.fanxiaobao.xyz/Article/details/gwdzejamb.sHtML

[S18] C：命令行参数
来源：http://blog.fanxiaobao.xyz/Article/details/ghhyfakhd.sHtML

int main(int argc, char **argv)
来源：http://wap.fanxiaobao.xyz/Article/details/gikmvxcsr.sHtML

[S19] C：快速排序
来源：http://mobile.fanxiaobao.xyz/Article/details/ggjhdgccl.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.fanxiaobao.xyz/Article/details/goivhhvmi.sHtML

[S20] C：二分查找
来源：http://3g.fanxiaobao.xyz/Article/details/glbbmhrte.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.fanxiaobao.xyz/Article/details/gmntgahnn.sHtML

[S21] C：字符类别判断
来源：http://3g.fanxiaobao.xyz/Article/details/ghboobhkb.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.fanxiaobao.xyz/Article/details/ghggiirzr.sHtML

[S22] C：字符串转数字
来源：http://mobile.fanxiaobao.xyz/Article/details/gzailsvnr.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcrlsapqf.sHtML

[S23] C：随机数
来源：http://www.share.fanxiaobao.xyz/Article/details/gatzartuo.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnzahadqv.sHtML

[S24] C：获取本地时间
来源：http://wap.fanxiaobao.xyz/Article/details/gugijijlm.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtunveokd.sHtML

[S25] C：内存拷贝
来源：http://baike.fanxiaobao.xyz/Article/details/guqneqdlo.sHtML

memcpy(dst, src, n);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtvpndwqz.sHtML

[S26] C：内存清零
来源：http://m.share.fanxiaobao.xyz/Article/details/gyaiwtfoi.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.fanxiaobao.xyz/Article/details/gydvfkiyj.sHtML

[S27] C：定义常量
来源：http://m.share.fanxiaobao.xyz/Article/details/gdgdhicrb.sHtML

const double PI = 3.14159;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzegcxmym.sHtML

[S28] C：静态变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gpshuhpyn.sHtML

static int counter = 0;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfmymgwsm.sHtML

[S29] C：变参函数
来源：http://blog.fanxiaobao.xyz/Article/details/gzqwdmcvb.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwzaitjxt.sHtML

[S30] C：头文件保护
来源：http://wap.fanxiaobao.xyz/Article/details/gehxmvcgb.sHtML

#ifndef X_H
来源：http://www.share.fanxiaobao.xyz/Article/details/gogfeozpb.sHtML

#define X_H
来源：http://read.share.fanxiaobao.xyz/Article/details/gnpdrmdye.sHtML

#endif
来源：http://m.share.fanxiaobao.xyz/Article/details/gwjwcroot.sHtML

[S31] C++：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gnshtecir.sHtML

#include <iostream>
来源：http://blog.fanxiaobao.xyz/Article/details/gkxrktkpd.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.fanxiaobao.xyz/Article/details/glscayqlf.sHtML

[S32] C++：字符串
来源：http://blog.fanxiaobao.xyz/Article/details/guxtqqihv.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.fanxiaobao.xyz/Article/details/glykunfsk.sHtML

[S33] C++：vector 增删
来源：http://3g.fanxiaobao.xyz/Article/details/guvlgtyyc.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.fanxiaobao.xyz/Article/details/gxycvvhfu.sHtML

[S34] C++：遍历 vector
来源：http://blog.fanxiaobao.xyz/Article/details/gzcyzgypj.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.fanxiaobao.xyz/Article/details/gpplkynzv.sHtML

[S35] C++：map
来源：http://read.share.fanxiaobao.xyz/Article/details/glszdffrq.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.fanxiaobao.xyz/Article/details/gvldipesr.sHtML

[S36] C++：unordered_map
来源：http://blog.fanxiaobao.xyz/Article/details/glithxgmr.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fanxiaobao.xyz/Article/details/gkuistdes.sHtML

[S37] C++：set
来源：http://m.share.fanxiaobao.xyz/Article/details/glvcxbuau.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.fanxiaobao.xyz/Article/details/gnwbkyqam.sHtML

[S38] C++：排序
来源：http://read.share.fanxiaobao.xyz/Article/details/gpakiabhk.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.fanxiaobao.xyz/Article/details/gpodgwfco.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.fanxiaobao.xyz/Article/details/gnescgrrw.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.fanxiaobao.xyz/Article/details/gsklpgrub.sHtML

[S40] C++：查找元素
来源：http://blog.fanxiaobao.xyz/Article/details/gfpdqtupk.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.fanxiaobao.xyz/Article/details/gqbkznlvc.sHtML

[S41] C++：类与构造函数
来源：http://blog.fanxiaobao.xyz/Article/details/guqimckuh.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.fanxiaobao.xyz/Article/details/gilfttjcv.sHtML

[S42] C++：继承与虚函数
来源：http://3g.fanxiaobao.xyz/Article/details/gcgvugvnz.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.fanxiaobao.xyz/Article/details/glndddbvo.sHtML

[S43] C++：智能指针
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grxtzrnlw.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.fanxiaobao.xyz/Article/details/gcgxbspkm.sHtML

[S44] C++：引用传参
来源：http://3g.fanxiaobao.xyz/Article/details/gnnnocxwl.sHtML

void inc(int &x) { ++x; }
来源：http://wap.fanxiaobao.xyz/Article/details/gtybksqcf.sHtML

[S45] C++：lambda
来源：http://mobile.fanxiaobao.xyz/Article/details/geosqccir.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.fanxiaobao.xyz/Article/details/gdqsfkulj.sHtML

[S46] C++：函数模板
来源：http://wap.fanxiaobao.xyz/Article/details/grsgnacdq.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.fanxiaobao.xyz/Article/details/ggndololg.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnmpfvdvb.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.fanxiaobao.xyz/Article/details/gqfrofwsz.sHtML

[S48] C++：逐行读文件
来源：http://baike.fanxiaobao.xyz/Article/details/gedltqpnt.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.fanxiaobao.xyz/Article/details/gczgadacp.sHtML

while (std::getline(in, line)) { }
来源：http://blog.fanxiaobao.xyz/Article/details/gxnigckno.sHtML

[S49] C++：写文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gttzlpbuh.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.fanxiaobao.xyz/Article/details/gofynpjoc.sHtML

[S50] C++：格式化数字
来源：http://www.share.fanxiaobao.xyz/Article/details/gcstsrups.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyykilnqu.sHtML

[S51] C++：显式类型转换
来源：http://baike.fanxiaobao.xyz/Article/details/gpwyakile.sHtML

static_cast<double>(a) / b
来源：http://m.share.fanxiaobao.xyz/Article/details/gsjkxztut.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.fanxiaobao.xyz/Article/details/gkratuqme.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gipcyjvht.sHtML

[S53] C++：移动语义
来源：http://mobile.fanxiaobao.xyz/Article/details/gboetfyln.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.fanxiaobao.xyz/Article/details/gyhzqvlcf.sHtML

[S54] C++：异常处理
来源：http://www.share.fanxiaobao.xyz/Article/details/gfnkaamlc.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.fanxiaobao.xyz/Article/details/gazwbsrpi.sHtML

[S55] C++：结构化绑定
来源：http://baike.fanxiaobao.xyz/Article/details/geaufnxtj.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.fanxiaobao.xyz/Article/details/gtroalbgr.sHtML

[S56] C++：optional
来源：http://blog.fanxiaobao.xyz/Article/details/gkwlffxib.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.fanxiaobao.xyz/Article/details/glpppidee.sHtML

[S57] C++：编译期常量
来源：http://read.share.fanxiaobao.xyz/Article/details/gwujfztul.sHtML

constexpr int N = 10;
来源：http://blog.fanxiaobao.xyz/Article/details/gvjeqwwme.sHtML

[S58] C++：命名空间
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gldbydfoh.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjadzwksb.sHtML

[S59] C++：静态断言
来源：http://3g.fanxiaobao.xyz/Article/details/ggedmoybb.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.fanxiaobao.xyz/Article/details/gszvbvgnp.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.fanxiaobao.xyz/Article/details/gvrjfhgra.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.fanxiaobao.xyz/Article/details/gyucocmiz.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gonwzpxaz.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.fanxiaobao.xyz/Article/details/gmcpbluxl.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gxhzsrhyl.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvzvykrgp.sHtML

println("Hello")
来源：http://read.share.fanxiaobao.xyz/Article/details/gapontyub.sHtML

[T02] Kotlin：变量
来源：http://blog.fanxiaobao.xyz/Article/details/gsxqieemx.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.fanxiaobao.xyz/Article/details/gkozadkmg.sHtML


<!-- 参考信息 -->