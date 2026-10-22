代发 wailian999

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2rbnpssoe.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2dnhwrvqz.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2gjdhdyns.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2egnzfpnf.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2tgikwjkl.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2oxrinaqg.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2thxeyxbd.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2fyattoio.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2hmnbfvki.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2kllguuho.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2rmaoimys.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2mjrggkep.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2hrcjyciu.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2qjmxuivl.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2nzwlnotr.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2rbgoepvw.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2lcehjdpr.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2xykazkuq.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2etkwdkdg.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2avwgpyou.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2jkkctphu.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2awhhkjje.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2kvsqyzvp.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2uhtrofzi.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2omclslzn.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2uqismglh.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2vmzfrdli.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2akfoduqx.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2saifhlcm.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2uppsfymw.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2eyazfrwv.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2fvfmqefs.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2dadhxsuy.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2akwujkdi.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2mwkacvat.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2xdaklmax.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2jssvbfms.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2pjirqflx.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2zytjvidv.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2gqcsxolc.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2yafbdskj.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2conauvue.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2sfcfxkba.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2hkbyuhfc.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2atxxudxs.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2ktqekjgs.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2hnioplfr.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2rzstyrbh.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2mrcarvff.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2kyawuxqr.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2uicbsmmp.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2wajglhmp.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2fozzmqfz.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2nqkyobaw.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2woglgsks.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2tckkyfsi.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2ffhkgcfs.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2kkdxhlbc.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2ulzglfxy.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2gbxjdpkb.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2mvlflynk.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2aqqnicxd.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2aetcdncu.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2guxbgoir.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2vnkizbwp.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2qtpqlbmb.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2ctmjvbwp.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2zwdudakj.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2qtvdfemz.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2hguagoza.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2jwedmjlx.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2cgoxdzuv.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2jxpjwxzj.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2pnmpjoos.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2fsycstdg.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2pdvqzqke.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2tohsvhyc.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2yjapzcfl.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2olrpwoqb.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2nlmmfqod.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2ejfbmblk.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2ngfsjcxo.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2fmcgfjcx.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2iynqfzbc.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2apcgoiul.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2yryagukk.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2fechlyoe.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2dnfdahxv.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2jdsfsnnf.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2eaugrzkq.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2hjznnoxm.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2vbbdrffa.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2nryepsxe.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2xrawxdxo.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2lhpqzcno.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2vbhwnilf.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2kbsygonp.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2ndqvmdfd.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2bjscetjj.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2oqiswefj.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2ascytlki.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2vbbupsqn.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2vkanntir.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2momqkmrb.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2kbovnuiu.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2fgiloczn.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2ywxplbtf.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2nwnzokjk.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2ijahpgbe.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2vjxhggdf.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2rmjlpmno.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2mjhyufwf.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2ebhnxiyd.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2hqkubkcu.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2ylhferjv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tdqfhpsw.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2esbadjsm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2oxhevwla.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2giwwkurc.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2bymjdmeh.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2prtmnqof.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2ftbhgbie.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2gaenexnp.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2pdumvnqj.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2bvqijoho.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2tpaxdvwf.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2lfcqwsns.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2rexnqllu.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2qtkvlcvd.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2hvcvslvh.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2ameozdyr.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2pzhstsyn.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2jibduply.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2fqiebxzo.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2vswzbljm.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2ezkamvpc.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2wnmekzqf.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2brqjpack.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2guxmhwou.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2mndjonyj.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2jdejlahe.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2xpytzsaf.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2prfzyrqj.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2bjhwnwcg.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2lrxkrdzu.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2xhtphqdi.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2vmbegakq.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2lxbgsxxa.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2hcyxssbh.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2xthwstgz.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2mxiidnxf.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2enyvkqym.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2msscqutk.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2thsfftpk.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2gercbxay.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2fjssnxgd.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2chscfszt.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2kkvbqvpn.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2pbtyxyif.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2rftrdnpt.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2adalbnld.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2cxomnhfr.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2oetrlfdm.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2jnerxaaq.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2oirjsjap.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2jfximymg.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2zgpfhces.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2qmgyiuvi.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2gpeocfka.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2aijdizau.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2sgudxnnx.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2cgzpowpg.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2creizzms.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2bqiqnsdr.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2hjkxcoxb.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2jgttizbl.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2sgcdjqid.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2ptoxvkko.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2tbglvedp.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2pwbiyxak.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2uynewzqn.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2zjwmnqqf.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2nmuzmmga.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2lyvelowm.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2rselvynb.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ouhevcec.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2drrsivwd.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2aayqeodf.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2nncjloab.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2bbmzhgia.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2rnihqebf.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2fiagxcsp.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2kshhbioe.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2xwdzhefq.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2ppfwezsd.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2lwgqhfbn.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2dwvcjblm.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2gxnkjxhl.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2fjhrvwdz.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2evfexbzh.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2nhrgajzz.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2vyiiuwgc.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2orcxbwio.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2gvbfjwwc.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2cvfrviwz.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2skgcswqp.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2wnnzniaa.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2skeuxgre.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2tbhgzpdf.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2ycknqnvs.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2ltizkfqw.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2fupnskfb.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2qhcklgrg.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2ulrqwhyx.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2fvzszpww.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2nlstsupw.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2lkmxqywe.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2jhlkaqwy.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2vqqipwnn.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2fsyrcabc.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2geqxoxal.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2kwgmqzga.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2coujsakq.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2miuahqna.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2tgluvdpc.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2ffayqdku.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2rpceffue.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2bbtwvsql.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2pwuymhpj.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2fdznzzvj.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2ymxfhgyk.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2kijporyd.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2qarkcsxz.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2rcxylklg.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2yzviryxk.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2bswsmbtf.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2aiialnxv.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2dnwxntzv.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2zncaxcah.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2tqbcadnq.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2rheujyvf.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2tydxcsah.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2hozhftfa.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2sasbxrig.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2oczguulq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mebkboxg.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2ctmcglth.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2scelbmml.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ymghhopp.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2mmftskhc.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2hcfflgqj.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2xjvhbwgz.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2qjtblkhc.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2rahlgehg.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2tcivlvuw.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2eepaentt.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2molwgqka.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2vhmnjfaq.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2luxmbcnq.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2aqwvjogf.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2prcuoadr.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2xdnaqqhs.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2hkgenrqv.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2rirrpqfy.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2ozwcnwwu.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2ajtiyqyi.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2jptqnakn.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2tbingbsn.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2nojxuhud.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2wkpivool.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2kikogsya.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2uslncgwv.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2yniihsjf.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2omfhtrvj.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2xvpnboje.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2jitdaumo.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2xodvmeox.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2odkptuqt.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2gmbfphuy.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2hfgkwehz.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2vxpnzxna.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2rlwwrcvn.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2mlnbfjkg.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2qjtqeiwv.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2psmpavud.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2yovlrbsx.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2yqqjkmnr.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2syprmdrg.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2foasaikn.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2iewykloq.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2gvqxmzch.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2kxfiqegm.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2fskkqxmw.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2njrbzier.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2uneldltz.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2nckspeuq.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2yldydjvf.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2lqvkjalz.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2ywkmvhhb.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2grahbgja.html


<!-- 参考信息 -->