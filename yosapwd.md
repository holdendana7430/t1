代发 wailian999

readonly PI=3.14
来源：http://m.share.zdbjq.cn/Article/details/genvlnvwt.sHtML

[R04] 位置参数
来源：http://blog.fehbvm.com/Article/details/gnzlqrqjp.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://m.share.zdbjq.cn/Article/details/ghmidypwe.sHtML

[R05] 参数默认值
来源：http://mobile.hesvh.cn/Article/details/goaekijan.sHtML

name="${1:-default}"
来源：http://3g.fehbvm.com/Article/details/gztidkpyd.sHtML

[R06] 判断命令是否存在
来源：http://m.share.hesvh.cn/Article/details/gsnauwdyl.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.zdbjq.cn/Article/details/glzdouscz.sHtML

[R07] if 判断文件
来源：http://baike.zdbjq.cn/Article/details/ghnwcttht.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.fehbvm.com/Article/details/gqwwnbgfb.sHtML

[R08] 数值比较
来源：http://www.share.zdbjq.cn/Article/details/ggaieopxp.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.zdbjq.cn/Article/details/gmkjeqzjn.sHtML

[R09] 字符串比较
来源：http://m.share.hesvh.cn/Article/details/gyedrojcj.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.zdbjq.cn/Article/details/gaoswxigq.sHtML

[R10] 正则匹配
来源：http://blog.fehbvm.com/Article/details/gpbowhifl.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.fehbvm.com/Article/details/gtemamvwm.sHtML

[R11] case 多分支
来源：http://read.share.zdbjq.cn/Article/details/gbuumvaqm.sHtML

case "$1" in
来源：http://m.share.zdbjq.cn/Article/details/gfappbtsw.sHtML

start) echo "启动" ;;
来源：http://3g.fehbvm.com/Article/details/gklhgfsyv.sHtML

stop)  echo "停止" ;;
来源：http://www.share.hesvh.cn/Article/details/gbusssvny.sHtML

*)     echo "未知命令" ;;
来源：http://baike.hesvh.cn/Article/details/gsjmzhqkq.sHtML

esac
来源：http://3g.zdbjq.cn/Article/details/gllmghrlw.sHtML

[R12] for 遍历文件
来源：http://mobile.hesvh.cn/Article/details/gulsqubdm.sHtML

for f in *.txt; do echo "$f"; done
来源：http://mobile.fehbvm.com/Article/details/gpnkruhhx.sHtML

[R13] for 计数循环
来源：http://blog.zdbjq.cn/Article/details/gvyevkqvv.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.fehbvm.com/Article/details/gbuxaynrj.sHtML

[R14] C 风格 for
来源：http://www.m.share.fehbvm.com/Article/details/ghbvuasgt.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.zdbjq.cn/Article/details/givdoxadh.sHtML

[R15] while 逐行读文件
来源：http://blog.hesvh.cn/Article/details/gvivawvmn.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.fehbvm.com/Article/details/gonaevzeg.sHtML

[R16] until 等待条件
来源：http://www.share.fehbvm.com/Article/details/gywvxegch.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.hesvh.cn/Article/details/ghwgzloer.sHtML

[R17] 数组定义与取值
来源：http://wap.fehbvm.com/Article/details/goaozsmct.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.fehbvm.com/Article/details/gkblxeoiu.sHtML

[R18] 遍历数组
来源：http://read.share.hesvh.cn/Article/details/gtfakzdpf.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.share.fehbvm.com/Article/details/gdjpspyws.sHtML

[R19] 数组长度
来源：http://blog.zdbjq.cn/Article/details/groyqcdzx.sHtML

echo "${#arr[@]}"
来源：http://www.share.fehbvm.com/Article/details/gxvmlnuds.sHtML

[R20] 关联数组（字典）
来源：http://3g.hesvh.cn/Article/details/gqihnjwth.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.fehbvm.com/Article/details/glybumksc.sHtML

[R21] 字符串长度
来源：http://read.share.fehbvm.com/Article/details/gtsuunjjb.sHtML

echo "${#s}"
来源：http://blog.zdbjq.cn/Article/details/gkxxehevg.sHtML

[R22] 截取子串
来源：http://m.share.hesvh.cn/Article/details/gtazjkbtx.sHtML

echo "${s:0:5}"
来源：http://www.blog.hesvh.cn/Article/details/gdqmixzrc.sHtML

[R23] 字符串替换
来源：http://read.share.hesvh.cn/Article/details/gahrchovt.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.hesvh.cn/Article/details/gsgrckpym.sHtML

[R24] 大小写转换
来源：http://blog.fehbvm.com/Article/details/gukoyvyxu.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.zdbjq.cn/Article/details/gftyrmotn.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.zdbjq.cn/Article/details/gbrynfttg.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://read.share.hesvh.cn/Article/details/gkxfbsbvk.sHtML

[R26] 命令替换
来源：http://3g.hesvh.cn/Article/details/gjkctdvhd.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.fehbvm.com/Article/details/gyzvpzsmn.sHtML

[R27] 算术展开
来源：http://mobile.zdbjq.cn/Article/details/gqqmkmaie.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.fehbvm.com/Article/details/glybwaljj.sHtML

[R28] 浮点运算
来源：http://wap.hesvh.cn/Article/details/gpagenyeq.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.hesvh.cn/Article/details/gzfiuuntp.sHtML

[R29] 定义函数
来源：http://www.share.fehbvm.com/Article/details/gkwpwgsrn.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.zdbjq.cn/Article/details/guiejobgs.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.zdbjq.cn/Article/details/gxjbfielg.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.hesvh.cn/Article/details/gtgddtwol.sHtML

[R31] 局部变量
来源：http://www.blog.hesvh.cn/Article/details/gybdlksqv.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.zdbjq.cn/Article/details/guqukyjlr.sHtML

[R32] 参数个数校验
来源：http://www.share.fehbvm.com/Article/details/girszwvga.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.hesvh.cn/Article/details/gvjcjrodq.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.zdbjq.cn/Article/details/godyyqlej.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.hesvh.cn/Article/details/gxhkvxnrz.sHtML

[R34] 退出时清理
来源：http://3g.hesvh.cn/Article/details/gmjjpipwq.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.hesvh.cn/Article/details/grdquqhes.sHtML

[R35] 后台执行并等待
来源：http://baike.zdbjq.cn/Article/details/ghjsksxss.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.hesvh.cn/Article/details/gcjrwqlwl.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.hesvh.cn/Article/details/gpvqyyjfh.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.hesvh.cn/Article/details/gpojswsst.sHtML

[R37] 把输出赋给变量
来源：http://3g.zdbjq.cn/Article/details/gyvnlaksc.sHtML

files=$(ls -1)
来源：http://www.blog.hesvh.cn/Article/details/ghzealdpl.sHtML

[R38] 管道串联
来源：http://blog.zdbjq.cn/Article/details/gsfoddweh.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.hesvh.cn/Article/details/gzfnpdbuo.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.hesvh.cn/Article/details/ggvdcxoyx.sHtML

cmd > out.log 2>&1
来源：http://mobile.hesvh.cn/Article/details/geafpchtm.sHtML

[R40] 追加写日志
来源：http://mobile.fehbvm.com/Article/details/ghocwupum.sHtML

echo "log" >> out.log
来源：http://www.blog.fehbvm.com/Article/details/grsxnyrtz.sHtML

[R41] 丢弃输出
来源：http://www.share.hesvh.cn/Article/details/ggviqykqj.sHtML

cmd >/dev/null 2>&1
来源：http://3g.fehbvm.com/Article/details/gnmutxajq.sHtML

[R42] 输入重定向
来源：http://3g.hesvh.cn/Article/details/ggsbqijgq.sHtML

wc -l < a.txt
来源：http://www.share.fehbvm.com/Article/details/gkbaqozjs.sHtML

[R43] 按名字查找文件
来源：http://blog.zdbjq.cn/Article/details/gwqefpbiy.sHtML

find . -name "*.log" -type f
来源：http://mobile.hesvh.cn/Article/details/gkfghqzwd.sHtML

[R44] 按修改时间查找
来源：http://www.blog.fehbvm.com/Article/details/gbecjirmf.sHtML

find . -mtime -7 -type f
来源：http://mobile.zdbjq.cn/Article/details/gmizpxypb.sHtML

[R45] 批量删除
来源：http://baike.hesvh.cn/Article/details/ggstwsyfh.sHtML

find . -name "*.tmp" -delete
来源：http://blog.hesvh.cn/Article/details/gounzzrxv.sHtML

[R46] 递归替换文件内容
来源：http://mobile.fehbvm.com/Article/details/gdwshmuxw.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.zdbjq.cn/Article/details/ggyzcpvdh.sHtML

[R47] sed 单行替换
来源：http://mobile.zdbjq.cn/Article/details/gslnyckza.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.zdbjq.cn/Article/details/gdcbkikwe.sHtML

[R48] awk 取指定列
来源：http://www.share.zdbjq.cn/Article/details/gcoercaqn.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.hesvh.cn/Article/details/grtubuysk.sHtML

[R49] awk 带条件
来源：http://baike.hesvh.cn/Article/details/gfmolkjpt.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.hesvh.cn/Article/details/grtlvaagr.sHtML

[R50] awk 求和
来源：http://3g.hesvh.cn/Article/details/gnynbouko.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.hesvh.cn/Article/details/gdfuohuml.sHtML

[R51] 排序去重取前几
来源：http://mobile.hesvh.cn/Article/details/gjkwitpsy.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.fehbvm.com/Article/details/grrkjggnl.sHtML

[R52] 统计行数
来源：http://baike.zdbjq.cn/Article/details/gzfauuteu.sHtML

wc -l a.txt
来源：http://blog.hesvh.cn/Article/details/gadetljtv.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.fehbvm.com/Article/details/ghpuotzkv.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.zdbjq.cn/Article/details/gzmdbsrfr.sHtML

[R54] 比较两个文件
来源：http://mobile.hesvh.cn/Article/details/gyofuever.sHtML

diff a.txt b.txt
来源：http://m.share.fehbvm.com/Article/details/gadvvzwbs.sHtML

[R55] 压缩与解压
来源：http://baike.hesvh.cn/Article/details/gmqlululs.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.hesvh.cn/Article/details/ghbaqtimj.sHtML

[R56] 远程拷贝
来源：http://m.share.zdbjq.cn/Article/details/ggjqspdma.sHtML

scp file user@host:/path/
来源：http://3g.hesvh.cn/Article/details/gekmiqkjf.sHtML

[R57] 远程执行命令
来源：http://mobile.zdbjq.cn/Article/details/gphzdcdks.sHtML

ssh user@host 'uptime'
来源：http://www.share.hesvh.cn/Article/details/gcdukufro.sHtML

[R58] 下载文件
来源：http://wap.fehbvm.com/Article/details/gnqbgdweu.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.hesvh.cn/Article/details/gzcjtnxrm.sHtML

[R59] 发 POST JSON
来源：http://blog.fehbvm.com/Article/details/gvutgoisi.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.hesvh.cn/Article/details/gpvztprpe.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.fehbvm.com/Article/details/gnpnwipco.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.fehbvm.com/Article/details/gjqvlnmpa.sHtML

[R61] 磁盘占用
来源：http://read.share.hesvh.cn/Article/details/gvyddxtpq.sHtML

df -h;  du -sh *
来源：http://www.m.share.hesvh.cn/Article/details/gmyqutldv.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.fehbvm.com/Article/details/gmgamltzf.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.hesvh.cn/Article/details/grgttnlxa.sHtML

[R63] 内存与进程
来源：http://wap.fehbvm.com/Article/details/gosyvllat.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.zdbjq.cn/Article/details/gjhawznxl.sHtML

[R64] 结束进程
来源：http://www.m.share.fehbvm.com/Article/details/gohedxaci.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.zdbjq.cn/Article/details/gtlanfjtl.sHtML

[R65] 查看端口占用
来源：http://blog.zdbjq.cn/Article/details/gmkshhwkl.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.zdbjq.cn/Article/details/gmwhnzman.sHtML

[R66] 定时任务
来源：http://read.share.fehbvm.com/Article/details/gxavsoaqi.sHtML

crontab -e;  crontab -l
来源：http://wap.hesvh.cn/Article/details/gkjhedqyu.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.hesvh.cn/Article/details/ggfpufhlo.sHtML

openssl rand -hex 16
来源：http://baike.zdbjq.cn/Article/details/gyptjmuui.sHtML

[R68] 计算文件校验值
来源：http://baike.hesvh.cn/Article/details/gbsptzucy.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.hesvh.cn/Article/details/gciarqkai.sHtML

[R69] 生成随机密码
来源：http://www.m.share.zdbjq.cn/Article/details/guphieiwo.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.zdbjq.cn/Article/details/ghdwlvkdv.sHtML

[R70] 时间戳与互转
来源：http://m.share.fehbvm.com/Article/details/gocsoyyoj.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.zdbjq.cn/Article/details/gqlruaxfc.sHtML

[R71] 日期格式化
来源：http://www.blog.hesvh.cn/Article/details/gjgkhjbks.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.hesvh.cn/Article/details/ggxhyjtqj.sHtML

[R72] 等待端口就绪
来源：http://blog.hesvh.cn/Article/details/gijwbubom.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.fehbvm.com/Article/details/gzixpukwl.sHtML

[R73] 分割大日志
来源：http://mobile.hesvh.cn/Article/details/gobdfpasf.sHtML

split -l 1000 big.log part_
来源：http://baike.zdbjq.cn/Article/details/glkfszoaa.sHtML

[R74] 批量重命名
来源：http://www.share.zdbjq.cn/Article/details/ghyumpbdr.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.zdbjq.cn/Article/details/glvxwgdcb.sHtML

[R75] 导出环境变量
来源：http://m.share.hesvh.cn/Article/details/gkkubdtuo.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.fehbvm.com/Article/details/gypjjqgei.sHtML

[R76] 使用临时文件
来源：http://baike.zdbjq.cn/Article/details/ghufdhkkg.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.zdbjq.cn/Article/details/gtkldafhi.sHtML

[R77] 读取用户输入
来源：http://blog.hesvh.cn/Article/details/gxjctmfjp.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.fehbvm.com/Article/details/gbberfpbo.sHtML

[R78] 交互式菜单
来源：http://baike.hesvh.cn/Article/details/gmjxnrcxt.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.zdbjq.cn/Article/details/grtclwilk.sHtML

[R79] 解析命令行选项
来源：http://mobile.zdbjq.cn/Article/details/ghcxqayie.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.zdbjq.cn/Article/details/gxpvntkeo.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.hesvh.cn/Article/details/gcwbkloga.sHtML

time ./run.sh
来源：http://blog.zdbjq.cn/Article/details/glsoabzja.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/ggtqjcfsr.sHtML

S. C / C++ 专题
来源：http://read.share.hesvh.cn/Article/details/grproqmmy.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/ghdvixtmo.sHtML

[S01] C：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/ggqolcxtl.sHtML

#include <stdio.h>
来源：http://read.share.hesvh.cn/Article/details/govsfifrm.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.zdbjq.cn/Article/details/gappjpxaq.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.fehbvm.com/Article/details/gzxhqknjt.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.hesvh.cn/Article/details/ggbnsngqt.sHtML

[S03] C：读入整数
来源：http://blog.fehbvm.com/Article/details/gmmitukpo.sHtML

int x; scanf("%d", &x);
来源：http://wap.hesvh.cn/Article/details/ghvlugwph.sHtML

[S04] C：字符串复制
来源：http://baike.zdbjq.cn/Article/details/gwgspctbe.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.hesvh.cn/Article/details/gghohqjxf.sHtML

[S05] C：字符串长度
来源：http://3g.fehbvm.com/Article/details/gqacehkqy.sHtML

strlen(s)
来源：http://m.share.zdbjq.cn/Article/details/grtnamjdx.sHtML

[S06] C：字符串比较
来源：http://www.share.hesvh.cn/Article/details/gqomsqyxj.sHtML

strcmp(a, b) == 0
来源：http://mobile.zdbjq.cn/Article/details/gduwaydva.sHtML

[S07] C：数组遍历求和
来源：http://baike.zdbjq.cn/Article/details/gpkjplmvd.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.zdbjq.cn/Article/details/gkqluqubt.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.fehbvm.com/Article/details/gskdjahyf.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.hesvh.cn/Article/details/grqxdblff.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.hesvh.cn/Article/details/gjjmxkebt.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.hesvh.cn/Article/details/gboqxurzd.sHtML

[S10] C：指针与解引用
来源：http://baike.zdbjq.cn/Article/details/gmumljiqs.sHtML

int *p = &a;  *p = 5;
来源：http://baike.hesvh.cn/Article/details/gfqnblkfs.sHtML

[S11] C：逐行读文件
来源：http://baike.hesvh.cn/Article/details/gzeetrklj.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.hesvh.cn/Article/details/gxlyurvee.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.zdbjq.cn/Article/details/gzncgrbmh.sHtML

fclose(f);
来源：http://m.share.hesvh.cn/Article/details/gmvukczys.sHtML

[S12] C：写文件
来源：http://wap.zdbjq.cn/Article/details/gvwomdgch.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.zdbjq.cn/Article/details/grznmhiwn.sHtML

[S13] C：宏定义
来源：http://wap.hesvh.cn/Article/details/gyneuyrbb.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.hesvh.cn/Article/details/gyyuuqhvr.sHtML

[S14] C：枚举
来源：http://read.share.hesvh.cn/Article/details/gjkkiggou.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.hesvh.cn/Article/details/gpbeareta.sHtML

[S15] C：类型转换
来源：http://mobile.hesvh.cn/Article/details/gsglqgdmt.sHtML

(double) a / b
来源：http://blog.fehbvm.com/Article/details/gytwtvtha.sHtML

[S16] C：位操作置位
来源：http://baike.hesvh.cn/Article/details/ghhcyimaa.sHtML

x |= (1 << 3);
来源：http://baike.fehbvm.com/Article/details/gxbyrifvo.sHtML

[S17] C：安全拼接字符串
来源：http://blog.hesvh.cn/Article/details/gunkemgjj.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.fehbvm.com/Article/details/gajjtdioq.sHtML

[S18] C：命令行参数
来源：http://baike.zdbjq.cn/Article/details/guskymdsc.sHtML

int main(int argc, char **argv)
来源：http://m.share.hesvh.cn/Article/details/gszblukeg.sHtML

[S19] C：快速排序
来源：http://baike.fehbvm.com/Article/details/gpifyqqrr.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.zdbjq.cn/Article/details/gzfesyyfq.sHtML

[S20] C：二分查找
来源：http://m.share.hesvh.cn/Article/details/gphxgwuvd.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.hesvh.cn/Article/details/ggfzbkvdq.sHtML

[S21] C：字符类别判断
来源：http://m.share.fehbvm.com/Article/details/gekhhgbwg.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.zdbjq.cn/Article/details/gudbbceil.sHtML

[S22] C：字符串转数字
来源：http://wap.zdbjq.cn/Article/details/garvzwyip.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.fehbvm.com/Article/details/gxxjtkcch.sHtML

[S23] C：随机数
来源：http://read.share.fehbvm.com/Article/details/ghdyoeflw.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.hesvh.cn/Article/details/gxmgcfdnm.sHtML

[S24] C：获取本地时间
来源：http://baike.fehbvm.com/Article/details/gfpapwyyp.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.zdbjq.cn/Article/details/gjywfnvfi.sHtML

[S25] C：内存拷贝
来源：http://m.share.zdbjq.cn/Article/details/gwffhdfct.sHtML

memcpy(dst, src, n);
来源：http://wap.fehbvm.com/Article/details/gyabpucuz.sHtML

[S26] C：内存清零
来源：http://m.share.zdbjq.cn/Article/details/gcakrzpvz.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.zdbjq.cn/Article/details/gsvrapzyd.sHtML

[S27] C：定义常量
来源：http://3g.hesvh.cn/Article/details/gulinzmyc.sHtML

const double PI = 3.14159;
来源：http://3g.hesvh.cn/Article/details/gwoyosgwq.sHtML

[S28] C：静态变量
来源：http://baike.fehbvm.com/Article/details/gzysklniu.sHtML

static int counter = 0;
来源：http://3g.hesvh.cn/Article/details/gwebtdvdm.sHtML

[S29] C：变参函数
来源：http://m.share.zdbjq.cn/Article/details/gvzzejzgi.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.fehbvm.com/Article/details/gunxmbrbq.sHtML

[S30] C：头文件保护
来源：http://www.blog.fehbvm.com/Article/details/ghzkjcqwx.sHtML

#ifndef X_H
来源：http://mobile.zdbjq.cn/Article/details/gjtgupudi.sHtML

#define X_H
来源：http://blog.zdbjq.cn/Article/details/gilddbler.sHtML

#endif
来源：http://wap.fehbvm.com/Article/details/gpabqkgpm.sHtML

[S31] C++：Hello World
来源：http://mobile.zdbjq.cn/Article/details/goztxbgmf.sHtML

#include <iostream>
来源：http://mobile.hesvh.cn/Article/details/ggpfqjpjh.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.zdbjq.cn/Article/details/ghpsajnwa.sHtML

[S32] C++：字符串
来源：http://3g.fehbvm.com/Article/details/gzoudqcjf.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.zdbjq.cn/Article/details/gdddwjvel.sHtML

[S33] C++：vector 增删
来源：http://wap.zdbjq.cn/Article/details/gcpifpkzz.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.hesvh.cn/Article/details/gazlfrhjz.sHtML

[S34] C++：遍历 vector
来源：http://baike.zdbjq.cn/Article/details/gsnsxxaky.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.zdbjq.cn/Article/details/grcvaxzix.sHtML

[S35] C++：map
来源：http://3g.zdbjq.cn/Article/details/goklmfwhn.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.zdbjq.cn/Article/details/gqrzuwfzd.sHtML

[S36] C++：unordered_map
来源：http://wap.hesvh.cn/Article/details/gbmmytxtg.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.zdbjq.cn/Article/details/gnniltfpx.sHtML

[S37] C++：set
来源：http://3g.hesvh.cn/Article/details/gzmehassg.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.fehbvm.com/Article/details/gensueefg.sHtML

[S38] C++：排序
来源：http://read.share.fehbvm.com/Article/details/gkpgivjqv.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.zdbjq.cn/Article/details/gsothbmld.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.fehbvm.com/Article/details/gvgnpdvjh.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.hesvh.cn/Article/details/gukccovzd.sHtML

[S40] C++：查找元素
来源：http://wap.zdbjq.cn/Article/details/grjgazrav.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.zdbjq.cn/Article/details/gpaiqnzlu.sHtML

[S41] C++：类与构造函数
来源：http://3g.zdbjq.cn/Article/details/gsirfjesf.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.hesvh.cn/Article/details/gabsqvxzj.sHtML

[S42] C++：继承与虚函数
来源：http://wap.hesvh.cn/Article/details/ggfcuqcel.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.zdbjq.cn/Article/details/gksyjxxlv.sHtML

[S43] C++：智能指针
来源：http://www.blog.zdbjq.cn/Article/details/gqnhesafp.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.fehbvm.com/Article/details/gtuyqbqms.sHtML

[S44] C++：引用传参
来源：http://www.blog.fehbvm.com/Article/details/gmmfhfnia.sHtML

void inc(int &x) { ++x; }
来源：http://baike.zdbjq.cn/Article/details/gkpebrqpg.sHtML

[S45] C++：lambda
来源：http://baike.zdbjq.cn/Article/details/gltsvzccd.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.zdbjq.cn/Article/details/ghzahgcfb.sHtML

[S46] C++：函数模板
来源：http://m.share.fehbvm.com/Article/details/grlezagcs.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.fehbvm.com/Article/details/gzeigxshp.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.hesvh.cn/Article/details/gxcqixlwb.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.zdbjq.cn/Article/details/gwksvdwpz.sHtML

[S48] C++：逐行读文件
来源：http://baike.zdbjq.cn/Article/details/gituszzft.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.hesvh.cn/Article/details/gunjhvqzs.sHtML

while (std::getline(in, line)) { }
来源：http://wap.hesvh.cn/Article/details/gwrlnbpoy.sHtML

[S49] C++：写文件
来源：http://baike.fehbvm.com/Article/details/gdhyohxjs.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.fehbvm.com/Article/details/gdrdntcgx.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.fehbvm.com/Article/details/ghjyszljm.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.zdbjq.cn/Article/details/glxdxamor.sHtML

[S51] C++：显式类型转换
来源：http://www.share.fehbvm.com/Article/details/gttldkqoi.sHtML

static_cast<double>(a) / b
来源：http://m.share.zdbjq.cn/Article/details/gfkforemb.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.hesvh.cn/Article/details/gwxbwrnsk.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.hesvh.cn/Article/details/goagzjgog.sHtML

[S53] C++：移动语义
来源：http://www.m.share.fehbvm.com/Article/details/gsfuzhwdo.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.zdbjq.cn/Article/details/grqqlwqhc.sHtML

[S54] C++：异常处理
来源：http://www.share.zdbjq.cn/Article/details/gkhstgtka.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.zdbjq.cn/Article/details/grwymyjrz.sHtML

[S55] C++：结构化绑定
来源：http://blog.hesvh.cn/Article/details/gfgmacijo.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.fehbvm.com/Article/details/gjeupgdmk.sHtML

[S56] C++：optional
来源：http://www.m.share.zdbjq.cn/Article/details/gfcwglipi.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.fehbvm.com/Article/details/glbhjeqyu.sHtML

[S57] C++：编译期常量
来源：http://www.blog.zdbjq.cn/Article/details/gfynwkzxn.sHtML

constexpr int N = 10;
来源：http://baike.fehbvm.com/Article/details/gillzkidt.sHtML

[S58] C++：命名空间
来源：http://m.share.hesvh.cn/Article/details/gbrrwnmrn.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.fehbvm.com/Article/details/grxosyuxy.sHtML

[S59] C++：静态断言
来源：http://baike.zdbjq.cn/Article/details/getbzpoao.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.hesvh.cn/Article/details/gjhcxoqpg.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.zdbjq.cn/Article/details/gwjfbhnxf.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.zdbjq.cn/Article/details/ghjmqgchl.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gekrziskj.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.hesvh.cn/Article/details/gsudkubjx.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gqizlfiwe.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.hesvh.cn/Article/details/gakwwrodx.sHtML

println("Hello")
来源：http://mobile.fehbvm.com/Article/details/geknnoyca.sHtML

[T02] Kotlin：变量
来源：http://3g.fehbvm.com/Article/details/gknvaetvp.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.hesvh.cn/Article/details/gpxhgeavz.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.hesvh.cn/Article/details/giiwxbtga.sHtML

"值: $b"
来源：http://www.blog.fehbvm.com/Article/details/gfakvpool.sHtML

[T04] Kotlin：空安全
来源：http://mobile.hesvh.cn/Article/details/gnobxckwf.sHtML

val n: String? = null;  n?.length
来源：http://www.m.share.zdbjq.cn/Article/details/gdefmujyk.sHtML


<!-- 参考信息 -->