代发 wailian999

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2xibiqswk.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2qcakivkv.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2sdibadnl.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2prkqcjmb.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2jihabazv.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2xvcbsdxm.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2evlczhzb.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2dorkbwge.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2sxnbtbeu.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2gsjylcmv.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2lfusajpa.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2ymgrueaa.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2tincyjrs.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2espybomm.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2bygjouid.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2qdrnlydk.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2fbkgieiz.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2tfwammij.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2rletnoyj.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2sdnmkzzj.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2wtpsoflg.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2naewzwxj.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2rohtkdrs.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2zzrglpzd.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2sihrgyly.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2vcflyrwc.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2dwwhsewe.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2ncqesege.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2twzuqsvb.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2hrcjrukn.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2nnmovsmh.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2ixvzneht.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2tryxeldg.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2iwzwqxtd.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2hxyyegpz.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2qkfjuemn.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2qvzmrfie.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2qxohzfay.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2rmeaztsc.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2veogusok.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2aimdfbkt.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2wiyirack.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2hknvahvt.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2ggtmstmo.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2byavvygd.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2vcadcdbi.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2aitedzoc.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2gqfqunxd.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2qossdkis.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2mogdpyrt.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2vijpwffg.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2nbqvrprv.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2znwkrmwv.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2nadkcecw.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2zfnwljnc.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2uqnfnsyd.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2lagsssly.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2cyhidgqw.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2egzpvphf.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2fjezijkj.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2gimuslqi.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2aensccpb.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2fujtwkvo.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2gkmpvzvg.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2yreilsch.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2vtgjhnut.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2slhlnksw.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2aovwcxxj.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2typjjxhi.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2oqxvjtpi.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2pzmesttt.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2klqdsbgw.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2orlqnrap.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2ripqiifk.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2ijbdeufb.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2mqqapgsl.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2qzdzrycl.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2ktpmrivt.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2gzyweugn.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2ayhizjqi.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2mcioalcz.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2vawnybmf.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2qpmoltiw.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2vpxujegu.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2lskcqqwn.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2ttvvnlqf.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2fkbimscn.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2slgsxsba.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2lqipjfrs.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2fnuucxny.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2rblzsgqk.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2jzltowps.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2bbyvwbvp.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2xgqoudqv.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2zupgvlxh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pyuimnbd.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2zetbqrhy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ddcgjupl.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ohndunco.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2zxkhsmxd.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2tnnszlix.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2xdnlmyom.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2ficedjyf.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2bpikpkju.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2buldzwah.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2nwbhjpup.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2ffycqtxt.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2wbhgtwbz.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2kolxqwcq.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2hhigzsqu.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2wqqksquz.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2bbnhyhwt.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2monybpmx.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2yyhdktte.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2xtyrostr.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2tawcwqbs.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2hekvxbkw.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2zegzfspc.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2hvyxydus.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2owkuxcbb.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2iubrnhjp.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2hpubbxhu.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2zcyruhuh.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2ebljpcgu.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2zwvpiypx.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2bnptuibm.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2pkmvsznk.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2hunnslyn.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2gcnzauwg.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2rattayic.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2zwvlxpnm.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2ftirvcvq.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2jpnwekpc.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2pglloaum.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2tsgaoghk.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2goaigzqh.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2awjqstpx.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2vmmdcyly.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2ayssjegj.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2kimtdoao.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2npinfqtu.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2gcrsnrii.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2qbikhgeh.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2ospquaop.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2njgagcga.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2fbcvturo.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2snfbnmtt.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2jaoajrhg.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2vwuzyrew.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2amobkbcs.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2tzuqosiq.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2gdnainqa.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2ezbokwrm.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2arsalvkv.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2xuyksbsj.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2vsrnjzho.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2zomgfpwy.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2ckbgjezp.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2buoldwsb.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2cowifyqh.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2uwgcbati.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2bqkmbjcj.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2mofvactu.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2lfbmeerr.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2otbqzwtm.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2ztsmovtm.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2brakzgpw.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2mvyfuhow.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2magtugus.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2kyhespjc.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2sbxtjsov.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2iydymsvg.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2ysexkynd.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2oryvpivv.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2yszdotcj.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2uuukmvgi.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2dvcfhplw.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2jepliise.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2wxxvfnho.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2xgbpjssq.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2fsbfjrsj.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2makwdunc.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2nvpvqyjc.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2ejjyhvrm.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2dpvjzrqc.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2tkqpecbn.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2rvsmvpcp.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2eoxvxrhc.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2xbgogerm.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2kybjakbg.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2pawblnuk.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2iwblaqll.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2ihozofww.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2jjtdmars.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2yyftnyel.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2zkuzpcrr.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2rwoomrdi.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2ynnljhfz.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2pafseoxn.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2vrqlyfdm.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2kepbxjiw.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2iydjdpas.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2zjqjombf.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2ionzuifz.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2cxbcnlbc.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2hqahroco.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2yjiikudj.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2kdtbsjxt.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2cdcwuwll.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2gsrdbfxy.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2zepszmpx.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2pbnvqqup.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2oizylqsi.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2ifdgjlki.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2pkzduwkm.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2csqqgaut.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2phutjeik.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2cgmcswsx.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2hxxrhryv.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2npbqzive.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2ziwqpbrd.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2smcnstah.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2jtriprbj.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2knuvmipy.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2vfayjhji.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kgxwxnxx.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2rkrmljvk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cgmawtuc.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2yzrlvnlo.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2zvndytey.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2lmhydtzp.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2tdyulqly.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2ypdafslg.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2zgjactxq.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2mpbvjvia.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2gonqeyfk.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2nqobtarm.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2jnyeovyp.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2vqguumoz.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2xktjhcok.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2nrxqcsdl.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2tbkqurtu.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2mmfvfppf.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2fvozeuab.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2cbsphkco.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2osskshyh.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2frttpcmk.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2semavcwi.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2czvxxrgg.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2repqafsp.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2jqfekdlm.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2zdgjrybj.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2sfflfzmb.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2uievrwhh.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2mvryjktm.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2xzinmqjs.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2zbciivni.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2ouqkxiyc.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2szhisczg.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2wxjeagtp.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2piuryfut.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2pdmesutj.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2kovydhfq.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2zxxmpsoj.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2fjuassfl.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2tnptjciz.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2lznagktz.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2amdsfqos.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2vfejqfso.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2uctloezr.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2gzjuocqf.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2foiqfzdy.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2bvlhjwnt.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2lhewfyij.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2knqzafru.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2scubctvg.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2ofzbfqqe.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2lqcuhrnd.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2rlykmkrq.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2wwjfvopg.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2nxgatsdu.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2dvljhpyg.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2acjsvbmf.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2yppkainj.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2qkikoakx.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2xmviuyxy.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2vwqiabrz.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2qdoggetn.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2nqhuuehb.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2gpezrkgg.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2oytickcp.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2dzkgzrnb.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2csimsfbd.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2fcuoesco.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2smkumsno.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2cmoqpkfg.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2roycubdj.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2issbriwf.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2dhdwefbp.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2fhzsyyqc.html


<!-- 参考信息 -->