代发 wailian999

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2muylukuj.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2dgrjrtax.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2upjkuxup.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2nnyhhnlq.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2xsxjiqww.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2mqbjhsog.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2ucxqweqa.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2rptisuwc.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2svpjvytf.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2hlphoufg.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2lhptiwbo.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2qugsikpm.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2xhtnvhmv.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2ekcwmtsr.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2htjoryne.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2dkfipaua.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2hjggxcgj.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2fnolkjgo.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2lnnynstp.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2fzlpjlhg.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2pcukclzg.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2cidjgwlw.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2gzirwmqx.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2blpchdin.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2joxcskii.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2orrmmfkb.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2ppcabncq.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2idexeoor.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2cqqmqyaf.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2twdijrjs.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2yicdwzfs.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2cygkmzfg.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2eqpmmyzt.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2ckbfuprj.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2ezvcrtwg.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2ozhjkkrk.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2mrylddct.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2jnxddyei.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2ukkaitll.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2pfkfbxsh.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2odsfuxpz.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2uzudzhmu.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2gunktcsj.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2ghpnmbwd.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2xusprotu.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2hrjwfsuc.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2ttrammzh.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2yjrgjlar.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2fddixosq.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2fwjrrgaj.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2bvgybues.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2dzgzsrwi.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2mapxflkn.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2tvebqwlk.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2bbvpfkkp.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2fczkcrcv.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2nbvxgcgn.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2nndwidxm.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2jdfkzofj.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2tszewtfj.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2zujyypff.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2motauxra.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2wpwevpvd.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2dihwixrk.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2hbpkcaaw.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2faieolnt.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2eojfjzyc.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2qkfsxcgi.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2pgalqxhl.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2lvbmimqg.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2yxbdtryo.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2vceyjnku.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2ooydndcc.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2wvuzjtwk.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2kyqekmsl.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2bnmzfbna.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2aftqlzfi.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2cumxirpn.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2googosfp.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2vlvxdkrp.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2brqglltk.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2itiigvcc.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2ongjemut.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2uvfpygfh.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2kjnutybb.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2mungkzpq.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2acnbcgnd.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2xqahwzpi.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2rzilgonn.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2xdayfrgr.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2nckmouzx.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2vmsnsohh.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2eyjjiiwa.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2murlgeys.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2gykwvqjx.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2devefdsg.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2fqmnizkm.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2yifdihre.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2hcpwcxjr.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2fguzqeaz.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2qnagegmv.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2bgjdykxe.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2nnlpnxni.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2slounugn.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2xdofgscg.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2byzbbuve.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2eyremruz.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2etraqnnu.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2xysyieed.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2yvkpzjpl.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2wezuipss.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2xfgkhmrf.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2mkxakeke.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2dqpgiovv.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2asvnzslp.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2tqmmonbh.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2jjkccdaf.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2jtrglsdp.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2lszenhjt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pkhahugr.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2kslidyow.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2frwrphjo.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2jennvitx.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2rmerqdpy.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2vkvzmfcq.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2ydambmhh.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2rzisojwd.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2vmsmemdz.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2ylnxcsuq.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2kpqpykxh.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2ivwngtqg.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2eniwglpy.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ghpbngno.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2qrdmilul.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2mvkcjius.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2fkihwkyk.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2eaeyiloy.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2xzgcclds.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2qjasvsma.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2ekvlyrhz.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2kchucdgc.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2fdhofyjf.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2yrlbmuix.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2avhkayhz.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2jaqcnjsj.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2lboywpcv.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2mrrfobbt.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2uvjbygst.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2vweggini.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2xaadhwmm.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2dyjvsmrj.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2owyhqhxt.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2npyikrvz.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2jchqcwwy.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2jkrlpdxl.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2olvmvkbl.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2tlhmnhgi.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2jshkuhmp.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2npgumwkv.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2ojhifzkg.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2tsihidil.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2dvptaass.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2gxdfmzfu.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2ufygipbq.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2mdazfiij.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2wzihuoda.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2giphanby.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2qheaedoi.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2yojhaosn.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2zddzfshn.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2litzwzjt.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2bgneuqcv.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2ultpndvm.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2zyigpnsm.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2txgfeuln.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2dflvelis.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2ibvtvyef.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2vdclrvvd.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2tlgdteft.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2dzokyhqq.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2xwqrtxxs.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2xopccvry.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2hpuqppkp.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2ubwzctze.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2jzdiiboq.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2jqmxtqkf.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2vrjhtrzj.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2rbkqbruq.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2urhlzovf.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2idbptbmr.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2iazspygw.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2ctxbvaba.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2drzwwrzk.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2aofxekay.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2nssfxzud.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2ocqgggjh.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2cwttxtnx.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2yunibmuw.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2qekurkqr.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2brrdtjwt.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2jthjwriu.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2jhnvukbs.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2uwrxrikm.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2qccdodjr.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2wnabtpov.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2ztcmlcvb.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2zlwwejli.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2izluxhkj.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2skiggacq.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2jrmigyjf.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2rkvueqfk.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2estpuqri.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2mxijtmst.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2ppgbchsu.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2prsrxsua.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2vylfrxor.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2plsrvmtm.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2kgolyonb.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2lsvojajm.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2mgbygzdn.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ajkitzoa.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2rkmqypfg.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2ywwfvzlf.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2kgswimrq.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2pkaxvguv.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2zarahroo.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2uxpjawxx.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2zwcyxzkf.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2uolwhzsp.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2woyxqaag.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2xcajqukn.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2vziheydc.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2ahiiugdo.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2nzjaonqs.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2kgnxkzvj.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2bkvilqod.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2ttwdoikk.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2vmkxtutc.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2bnjggqqh.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2ximddkrq.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2fctpcxpc.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2ajizrhem.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2ckspyoze.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2ladbkuex.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2jfxiuxqz.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2vvyxkntv.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2hctttnnt.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2lptjzdhi.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2jyqhtrfd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uikkhefi.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2wprshvsk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kbdizsmh.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2kpjrmetx.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2ypjuthzz.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2xwqxfoij.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2pdczetny.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2jhithkrs.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2bftjgxsl.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2clpfjnkd.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2ucqebpgf.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2mlijervi.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2torkdwww.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2nnamfvau.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2mxejnvsw.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2dtcmeodg.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2szvbqbqd.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2thkyctan.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2rsotrchk.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2tkksxygr.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2wmbyvwik.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2xaybpimd.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2bdbnevsm.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2bucpwyfq.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2wnxjqvpj.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2rletrfzm.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2pajemsvb.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2jdoijnfw.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2pmlccetu.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2spebtvby.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2zwpoxvqg.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2ddsqhagc.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2dnmzsjvk.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2eiffatff.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2rqsecvef.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2vfshkxop.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2bpyiuolt.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2oikngcpk.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2uuplbrae.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2sdgytjhj.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2mftpjnun.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2hybpuplo.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2vlvdnito.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2bdombpka.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2egexwwhd.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2mhclywyu.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2sgavrmdi.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2xeiuvuqj.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2hpkhjocy.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2pdiwgcrl.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2nfkuvrvt.html


<!-- 参考信息 -->