代发 wailian999

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2loqtcmlf.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2fecvnoil.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2ryhflmjf.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2gormcbzc.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2tcvfcqak.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2ygrafnhq.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2lidnwyjj.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2qzrqfrga.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2blohzjdy.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2wqydrkaf.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2gbuxuaub.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2ugnqksma.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2hjftrwvs.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2rrtpanzi.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2efwtoqlp.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2lnxohqqx.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2cvesmujd.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2nhdvmwcg.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2bmwgkjdc.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2yzmrlzxu.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2cnkgfrij.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2ozcatuxm.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2jjojdezu.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2sjkofbzj.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2qpksjqxr.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2dhttwxbu.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2axpttvpu.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2wcdyhbin.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2gpvwtxki.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2yvwxguas.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2nnwpcolz.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2fyzfbouv.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2nfzlbxnz.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2nppmckdm.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2dvqensqm.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2jnpiyrne.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2rckemyma.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2pxmodwyn.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2dwtuddzs.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2gsdfmkqb.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2hxqrfwkz.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2fmejjylv.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2ujnczxoq.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2kmfgnteg.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2yklpdtaz.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2djnhhkps.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2deojzves.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2acsyqwmd.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2awtsdmeh.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2vzsyxohb.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2upkhyfzv.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2wzyznoxp.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2ithixfyk.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2egofntio.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2gcbllhxt.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2wkixifxg.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2nywhhkhq.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2ezfskncl.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2zrlxhetf.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2zkqobvhi.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2aysgjmni.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2utapnmdt.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2iymyryft.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2mpxbdarv.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2imzfzzyr.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2nojlsyxi.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2vfwkhmti.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2fzbnsnsx.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2hggdqufi.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2umckoxim.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2zmcvcwik.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2birjkvvr.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2ziomknkn.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2pnraehnu.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2cvyduptc.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2lopvjtrj.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2msiueopy.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2fchyesse.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2wlwimodj.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2creeurhu.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2pcskxcsd.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2ktzgvxgs.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2srakkqhy.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2nszcctej.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2rpfvxgom.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2vhgwqrms.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2kppcbtgy.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2xlwlcbcg.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2sfqresaq.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2ieqzumvh.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2pbthzphs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2blwcuwce.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2wmmctuqa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2efzsxsxf.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2owzicgwl.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2yofaxjzv.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2jivlniwl.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2twwbwnkm.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2ahfbkkrq.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2hkcamrnk.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2llolqbvx.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2ypfqblif.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2mebqaguu.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2babngist.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2ynusitlr.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2gmnoghah.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2pwdspdtd.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2grbkzpet.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2riesojai.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2jserjruc.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2szgsctnv.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2gdkmykyu.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2ihqlgsfs.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2gvnpfvwb.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2adwveivs.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2wcdynwgc.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2znbkroyq.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2ahxrycke.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2asqyscyi.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2rziygfkc.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2bwlsikgx.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2ehltfqay.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2sbyvdkdo.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2iovtcgjl.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2keweeekl.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2sfodebjp.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2rkdnmfgv.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2kucwhlzs.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2fcqphpxw.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2ebuifprh.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2pecmyhwc.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2nhgllydy.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2dwnkqotq.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2pwaemmsj.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2jzsmjbzq.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2ssawhrtf.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2mvlcfuwi.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2lspwpuii.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2facjdacn.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2ybmnodjz.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2gdadqqfn.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2etbhphha.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2blavhnyw.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2mralsolw.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2iprhawyk.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2ltyyepei.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2gffckonl.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2anriolxa.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2unvosetf.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2bsujmirx.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2ugmdtjgb.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2leyprktd.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2qfwjtwur.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2lrqcthzm.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2piravueb.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2xtzzvvzq.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2qrhsnjfm.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2zzigphvm.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2nxmjfsbk.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2qyuxczir.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2znuhrtro.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2hkwhhmkc.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2rblsotmq.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2jnrrztoa.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2ujmmmocs.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2cqlsqlnv.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2aehsqrng.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2pldftpyn.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2mtxccaaa.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2oepcyokf.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2awexquny.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2ulkscwlw.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2jemlouji.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2ndslmwnv.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2wgucmhui.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2wjddmikq.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2kumprbtk.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2hkceewlc.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2rzyoiltp.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2tayhnfwt.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2jbsjqhyj.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2xizmzobp.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2pukgxkqq.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2fvmmeana.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2wvonggln.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2gzpdfbgy.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2roqkjbot.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2hcrksief.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2ivhrbzfh.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2kygrkkur.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2jszzjiyf.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2eiijfuuu.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2qvuxwhor.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2qnozyevi.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2eykwiazm.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2dagundck.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2vcwuaafo.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2uytioxdx.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2oqshfcns.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2dzubdicl.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2xysqvzrw.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2cqixzsok.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2hxnttqca.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2nuengdyr.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2qtzjyrko.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2ynofoxve.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2oyvsqjru.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2sufdkmor.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2yxpmwvwe.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2bykmmzfj.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2dlshimrv.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2hfldyzmq.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2cngmwwzo.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2wtpzmdzc.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2lypjfezj.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2qvdeluwm.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2qlbbodyv.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2xfjsaasb.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2dajyulyi.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2lwtjomzn.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2bqoulorl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bprexibw.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2idkwwdal.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2stcfnzaj.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ywcevglp.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2jykagxxc.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2gltenyfv.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2sqksapbz.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2fncngjxu.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2afrvrafh.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2ebagzhoz.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2jzxnaogi.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2lbriwohw.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2qnuyxldt.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2ticskxwt.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2dshmkpph.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2xnruggap.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2gbihwfzw.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2cfgovdpr.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2padqybvn.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2aegrboto.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2halgttvg.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2qyhygctt.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2sjiezbqr.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2tywllrgt.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2nejohfjs.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2jvqbhusn.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2iwodatyd.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2gkunmkaf.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2quearomc.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2hneuoqfz.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2smlwksch.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2vtkkgqke.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2tbldfbby.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2lllwvsrp.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2dkjxessr.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2kypjfezf.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2oywimazn.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2peuhkyuf.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2nujfdklb.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2aatwzdui.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2yamumczi.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2cpptdttr.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2railslzb.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2syduayde.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2rpacrctg.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2mptmhyne.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2mjhffyax.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2wvkffdzu.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2yvmvvmye.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2gthbzusz.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2kmaeyxcd.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2poajqulq.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2dforwyku.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2gepsmbzz.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2yziqpfym.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2kpzolllt.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2kpftykfv.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2okkjjukd.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2ncjcojyg.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2tfbmkvst.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2eovsuroh.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2uizsqxwc.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2cfzzrhje.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2vrfcwiod.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2ntbncdvk.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2czloyggr.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2cdldvqbk.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2qwbxsvig.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2spqgrvhk.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2htmufxqj.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2dbjmdoir.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2ovwsrjix.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2dounqyzp.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2ptsammgz.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2xwjcvzsh.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2dsvtdpnw.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2awelogii.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2iulojfxf.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2jbsdlsfk.html


<!-- 参考信息 -->