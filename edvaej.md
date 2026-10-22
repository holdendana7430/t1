代发 wailian999

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2hhatrjfz.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2kgitzhog.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2adowlggv.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2hviqilvs.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2thmfwqkh.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2ozscihiw.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2wyneywfk.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2lubbbfkz.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2vivdfhou.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2dnaosygu.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2psokyonw.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2qbtmmdiu.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2cmxhjuso.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2ayfyrbxv.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2vcoolstd.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2ckmjvkyy.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2ovlqdpiw.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2ifxlijbb.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2cxozbldq.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2ebkzliol.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2cdbwbyjs.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2nthxyohs.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2mmbgeyfh.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2dafnqggs.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2tqwwxmps.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2jifizody.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2pxwebaqx.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2xesipbqx.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2nikxuwmb.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2kwtefsco.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2oflgulzd.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2rxfmubdt.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2nnxqzslr.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2ycutkxov.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2gvpyogzi.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2pssqqcmm.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2vfvramem.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2hnnkaylm.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2vfrxwrtr.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2xeocztbt.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2bxwkzhce.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2wvzngghf.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2ltnpkbia.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2wpgrmcxx.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2ukexjmwi.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2wqtzxybj.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2kxbzdxui.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2htagoibr.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2kvazlqzx.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2buwjnfdc.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2rexodijx.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2tpwsaiah.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2mukuqmtt.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2kxzojbsi.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2hssxbokn.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2bpmiodww.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2gsqirjrq.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2beicklij.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ioodjnxm.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2uvcoxmgp.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2oqcjdieo.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2inebncan.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2vtcvepup.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2fgsaxqky.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2wpqfcfgz.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2oagbtrxe.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2elbjaryb.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2pbdutkct.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2hdimizga.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2rrthroau.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2degmmizr.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2gsvvyfag.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2enlqgkyu.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2ixunntjd.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2divxwtiv.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2vinzjkqb.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2nytmrloi.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2ebyfjxpm.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2ingocajs.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2ffcambpr.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2pcbvjuhx.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2mhxnczyk.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2fmygwaam.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2zlhmrjrg.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2ouhniodd.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2acnssdzn.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2xxtxqual.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2kxzidxsa.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2smeorcdw.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2moezoccy.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2tywmujcl.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2yxbloden.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2bwbvtwfa.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2vpcmvpko.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2mhwkpuad.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2lvgipvjd.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2ijcrnexc.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2hevpxwkz.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2olxnmmce.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2igvzbhrq.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2sxooiqme.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2zadqdngt.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2xdnxugbv.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2uqxjferb.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2wmnujdpt.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2mvbpfiri.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2ivsjpgdj.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2pouqlhlj.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2fffiflpe.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2vvhtwmvq.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2wfvgkwjc.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2zczvdmhs.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2ezicexig.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2ympaqsjs.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2ujznvpsu.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2qsnxfqpw.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2nrrzolnu.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2kpwjvbds.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2wjajsgeg.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2azwhzngl.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2stkjwckf.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2xwkgnvgd.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2grsbqaxq.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2usgasnih.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2rjvzacvb.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2kqpmvokc.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2xbdpqoqg.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2vxdmlegs.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2gwraewyn.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2mnehnorq.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2abqhnjrn.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2fhjrbmsb.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2hkuxudyd.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2qplevnht.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2buhlrfaj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nfysyeld.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2wzkuiuyb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2iswxncve.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2rdpbxktc.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2exrtckhg.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2fwuhkmhd.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2gcvgmqso.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2gtzijqiu.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2cwjdxrwd.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2fizmzkjs.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2onyubfvg.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2ninvrelh.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2grniptdh.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2aorkkhbj.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2rsmlivic.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2aynzhnnc.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2hcukvwcg.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2onvpfeuk.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2jctbkybm.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2pzuhnkxo.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2xctfzgtx.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2fngjoufq.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2pvlxrkhg.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2qwhiulbk.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2iyemoskq.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2ghkymymg.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2zmwiiehn.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2wjnethgg.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2rskdduzr.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2zzcadgpf.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2fbgfwnvj.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2shcrgkxl.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2sfdahfjp.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2kqjyznez.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2syqxtlux.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2osadzwgk.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2olipfycu.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2oewhxhqv.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2zumffdgw.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2vwzthjju.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2wpdjnpqj.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2bxhwkiaf.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2owqaigvu.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2kvrzpeiq.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2sgaufyuo.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2wmvwyqie.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2iopbrneo.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2gchxchir.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2twkatlzq.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2abaepwga.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2xhnrbqze.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2zymdnygn.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2jvxnyhhq.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2mxizhjzu.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2ahddtznp.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2bngmywir.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2ydnyrwhy.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2qejazdfu.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2riqrztxj.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2lnbjngov.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2czexifim.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2dgcmjocb.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2aylqeiij.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2iopvnejp.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2bgbuwvva.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2bmlvyznc.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2xghpctvf.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2fbylqtkt.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2hywgboav.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2lntrtcet.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2slmatbng.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2cajsehib.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2cqsrsphd.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2wuaxawpl.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2dljqaqnw.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2mazsovpn.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2gllouosv.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2pwiswzot.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2eolmbzwr.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2ybkjztqe.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2fclqjsci.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2lppnrmts.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2uoresvso.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2paermqnf.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2svvhtiua.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2hznrupqp.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2rkonssbu.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2xnzcnltg.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2ykzoxban.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2temuwsbc.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2hplhaglv.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2lkcxhxxa.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2mfbiqlrd.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2davifhvg.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2qpdnintq.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2ugektbcj.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2gchusiui.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2jizrncvb.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2yjekzezd.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2ndoiulyz.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2cfhchquc.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2mzrdmzby.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2yukqefzo.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2uwfpyawp.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2ttjdptpt.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2pesqtynp.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2yuvhautf.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2dajgdzng.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2nzcpuwjt.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2zbnjfucj.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2qzwwdyka.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2rlfiukho.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2frdlcsdy.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2rzlcdwja.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2qyckcxid.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2uaqwvolv.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2lpbfgddd.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2wbvrlnhe.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2lnqsxyhy.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ibrqdsxh.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2sfxibcau.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2bwlumonp.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2szkvdxql.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2urizvlra.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2crjbpwps.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2apnykveg.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2sgwuwifi.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2xvoahfxt.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2bobanaat.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2ssxhquhu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2suswdjwv.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2zhkxnebi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yagsxcjy.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2awtodznt.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2ruxogtrp.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2qwfrzcpf.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2fyjpjfbc.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2omfpioum.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2kpgiqcth.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2nmidadkc.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2kutlshpl.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2goakfuyz.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2vrxdllhw.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2mhdadqbu.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2eqernujm.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2dwwxgjoy.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2rhenhiqg.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2cfrhfacs.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2xmmfzace.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2wskjcwhy.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2wgedosca.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2mkwhipnz.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2edxiupcz.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2hogmipgr.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2lxhcpdwx.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2pckehaeh.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2hrraohhv.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2udfeavmc.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2qjroztlq.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2namphrsj.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2xczkpliz.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2vpaorzjk.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2ngauyita.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2fwkdrytg.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2idqpliqq.html


<!-- 参考信息 -->