代发 wailian999

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2ayvbqsih.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2xnellite.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2yaxdnfsy.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2xmqqvrtg.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2tkootmiz.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2myapdyan.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2dpbzthbc.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2dzkqyjzp.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2xnwvdtse.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2cszuvylp.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2ifsqpglq.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2pxyiunxp.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2fvbyiehn.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2lwwwejkg.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2uefuegrq.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2nlbbfria.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2pmtqmaxx.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2xkruxxev.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2yriahtjx.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2tljnusqe.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2lzzwbnuj.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2aiyarhid.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2bacrdihd.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2dlicyjjg.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2mlstzqhk.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2tbrjixqt.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2xrscxbcq.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2cyeaotxj.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2ycoezatm.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2wbkfmhpn.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2jdhzdndu.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2subcgtpr.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2skakuyxv.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2ozmmdone.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2ahddrwnm.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2agskguhk.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2klaeyygk.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2nioarwcp.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2famiiklf.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2gprsjucb.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2vdtctdoq.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2mzqvswfa.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2dgxzqnnt.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2jvmcvxcp.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2novuxpmx.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2qpavofga.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2umeacthy.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2lwoeefla.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2yqmbpruh.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2iftdpmad.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2rlmqvrvx.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2vmsbycdp.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2nwbcetfo.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2jdfannfr.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2gxeeygfn.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2irwfvmpg.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2lfoxishb.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2ebretulw.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2jurxcwzt.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2ehpkkyya.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2meeilota.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2buupcwsz.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2luuqzzzh.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2odfdejad.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2wnqctkqj.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2rnsodzva.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2zapdepxb.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2lbjznaed.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2reutqqji.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2qcyrmxdm.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2nzqlfblv.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2lqeccdyt.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2sjdjsayd.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2guxnebyp.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2vaywtwjn.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2gjxsjgha.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2kbfdwjfs.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2pmcrhspn.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2gailxtxo.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2ubdrmxan.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2bjeqfiwh.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2rtnldrmc.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2hojcdtsp.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2gpaxfesd.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2obshfvpn.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2smtrmznv.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2wrgtzenu.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2bbgytyyl.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2onyxjpxt.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2bxbambln.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2mqcyfoba.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2ouljeffm.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2fxkwbjqc.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2zjjtlebl.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2oknauquc.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2zmhjrvsv.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2uqxbmcop.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2mchrrkxi.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2hpliyydh.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2crcenkjb.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2yduprlfi.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2ixhnabhk.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2unmbjghr.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2ixljzzjb.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2wscmiakj.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2zixohrip.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2kccmiejv.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2yzhayvyd.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2odsgnjup.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2jvrslosz.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2gofmhjqr.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2otihbfau.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2xbxrmrps.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2gqnitwcl.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2gmonkaug.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2kyhjngdb.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2xcdjxsjb.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2vpohuzfe.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2lntgcubo.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2zxjkdisz.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2liyqphxh.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2xrpuvcsh.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2uhriimgu.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2qchkxwfq.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2kwyeuvll.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2sgxgzjqf.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2rkchzqpx.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2mjvmxmpl.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2sqzigdas.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2hnkvellv.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2cagvvnfi.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2szgfghgp.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2eczlocih.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2rhdtbtik.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2usovwfug.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2eflprcwl.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2batqtkhl.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2hjkaqxic.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2fvoceoqc.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2xufrpdfa.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2dhirinnk.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2ixswqgfi.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2xvmjtfej.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2lndrfian.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2ndsfehuo.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2kfwkkkon.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2hvcszphy.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2qxjgemln.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2ktczebxj.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2powncqlx.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2ifdrdrya.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2tvdpwctp.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2tkdhglcc.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2fmwgwzpi.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2wfseuknq.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2ebmsjpky.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2icnsecnz.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2gcjjejwe.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2hdsotoyf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mcnazloj.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2reichjlm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ayxlrftp.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2gxqckadw.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2sqesytsz.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2znhvoxhb.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2zzazzlcd.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2kkqhxwmw.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2ipjooonl.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2uullbihy.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2ufgmydwt.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2wpwzvvxg.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2vhfefons.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ilhuyemt.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2kceeeqxg.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2iibaqjot.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2pnlengwl.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2wknojapt.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2olzidyhq.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2azukijef.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2wecijkyd.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2dxqxouab.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2zhhcgxfy.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2lsssifrz.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2ktjkxfzg.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2oiqiidue.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2pihipcjo.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2jcdfxuyg.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2gtvsflsi.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2bdpqsjwc.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2emhlofps.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2ryfwhmja.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2scqbenkg.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2sxogeqjb.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2sjnlknvo.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2qywyqjov.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2ezznyesg.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2mwmjzfsu.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2yphzadlt.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2rqiswkln.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2pxbmwgdm.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2bzoalldd.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2gfdwbgsy.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2yjrodgxm.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2peviidak.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2bhauskig.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2vnetxqum.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2wctqiirr.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2livqfyiy.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2bqyrqefv.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2ebgiiffh.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2qehibxaj.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2wytxtcmr.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2ufirijwz.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2njfjkmts.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2qakyolpc.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2xabvhfmt.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2yiwhtzzm.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2remfpyjg.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2fvcfdvne.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2fukhkxzo.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2vefqswnl.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2aldjuqts.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2zccavmvj.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2uiiqgqac.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2ojfxtpam.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2wgkennqp.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2wwimrpna.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2zebgykwi.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2deromvcz.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2pghfaewl.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2samuriop.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2glpmlstb.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2mfvocbzf.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2noysqotr.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2qkzedhtj.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2boqwqqoa.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2equdovif.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2qtxysmvo.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2umrvjrmt.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2kaawzghb.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2lebjdggd.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2tzwcbegh.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2nyfcdbej.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2zdnxminz.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2aueyyqcn.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2vhwbpprq.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2pprjpvdp.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2cibmvqnz.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2wvipbuqx.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2bzbzuhja.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2cytgyeui.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2etkiplqe.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2xoatwuws.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2gsxgjqqa.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2tzujmtcu.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2zqkxblsj.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2rrsurbzd.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2udqtbuzt.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2rnydkzvo.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2dwhllfka.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2iribusvx.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2xhblksdr.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2iqffaeef.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2pwudjltd.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2omzqpiaf.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2pwbczewh.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2rtlukste.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2nygiafzx.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2yqxexhiz.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2sxkpjdzz.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2tihbgmdy.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2tuukdkcj.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2ypywbdcx.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2sukutigr.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2qldejnnq.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2eflrewpa.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2qzmclhfg.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2qlulpzku.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2tbftwgla.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2ltrkyptg.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2jorxmbll.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2izpgfvtu.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2btegxetv.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2fwejracn.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2dlyzzdzc.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2aoykvxkf.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2qchpzrsr.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2pnohmbhx.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2vnouvdsl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mduokbyf.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2mlyslurk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2olurfewd.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2jfronqua.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2hulhbiod.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2wkpffazo.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2nlhyxbsk.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2aqbedskg.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2xigpxkyu.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2kxhntxfp.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2ooklifnc.html


<!-- 参考信息 -->