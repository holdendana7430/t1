代发 wailian999

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2tidybqgg.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2wkwhbuum.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2xgjpcdaw.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2zmqhgojv.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2syxvwknm.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2onalznjy.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2ypsnohxg.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2mklizrta.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2iqocueoq.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2igylwfjv.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2jyvyaphp.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2ihuaposu.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2yqgzyjeg.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2savdcoew.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2tvxmayab.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2tkychiwt.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2ynudqssz.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2ktgncilv.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2dyysjodp.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2kyzgpgqb.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2zcbeceaj.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2ohtcyphx.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2wwuhbdrz.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2pajdhbpr.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2tvgaftte.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2sakkcwhk.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2yksmdjit.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2fffwuvtp.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2mapmnhpb.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2abulaany.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2hqtinymj.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2gpbhtalj.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2yrutzntw.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2ktdithuc.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2rmasrxud.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2wmbylkxt.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2scxvkzln.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2llsbgnqr.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2gvkmdxxh.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2dapovjnd.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2rrphqyzb.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2fwhktwrw.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2fiabiaxe.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2ezsjrktj.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2fwkgfahw.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2imrxuuiu.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2dcskjnmm.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2lwjauyir.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2vvvhbxey.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2ukwehglc.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2scwgjdkl.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2evxoaupw.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2uqgbiecn.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2exzixvmr.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2vwnoajpb.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2aoyfwwlv.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2smsjrrhs.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2liqmkvnq.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2mvilahmw.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2sukeorxs.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2qthstfbm.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2cqqanslw.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2qpnxahaw.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2szejtkpg.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2xwqpoire.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2qmdfvioj.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2sycvpfxh.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2daeozaik.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2lwwsobat.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2jcmmpjjx.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2hkmifhef.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2jvfocdiu.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2cjvnrryl.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2xosbkrjg.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2uxejaejd.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2xxufofil.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2apnykrvs.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2eetwtqpn.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2oiaonqrh.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2adlusarj.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2umxjkmsk.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2hqsvhbos.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2wmsceegt.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2lkiducxv.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2ezmxmgpl.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2nbrxxmey.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2zlfoxseo.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2rehxakpn.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2pmsoabpo.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2ikhqnqpp.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2fkyeypbe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2noqgsogt.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2iicmbdht.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gnbuxioe.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2jykblzdf.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2hdkfntis.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2qnqwhrpp.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2lgwomxtt.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2wsyivufi.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2slkuabqk.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2eoibdkvv.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2grrwkscf.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2rndqjhya.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2bdxxnzqp.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2nbgwwyrg.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2xvmgljjz.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2tikoxqnw.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2vvcpditr.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2qswivkzy.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2ehgnrtpv.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2hubqiuhe.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2oahegmli.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2ookrokbb.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2bhwagdco.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2szsnbvim.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2akyecgfb.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2jxpdofkm.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2jjfyuvsl.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2qdwqvslx.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2djbdyaru.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2lwjqnmzi.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2bopbxnfe.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2bnzviikb.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2jmykkmpd.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2odfxrmsp.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2vudsofay.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2jdycbhvm.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2rzbdwenz.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2sbkkizbj.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2kxnyvxae.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2dbqegjaq.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2cpzrabqi.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2tiugotgx.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2zlxvykcg.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2ecicuhit.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2vzxwysiv.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2gdwpxqko.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2cecswyvd.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2mawpoyxv.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2wihstwkh.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2mznhguok.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2iiwvlejk.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2rhyxaaod.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2kuvzziir.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2zozvgkrk.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2dufnvwfa.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2bdgdktus.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2jaxneasg.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2ftmntbtc.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2hgimcswl.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2cgjfqkmt.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2lbqacsis.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2ufqfiwrn.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2etwfqrik.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2vqdvmkzi.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2zaicyexf.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2wycutpne.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2ulfplnsa.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2rtdkrbvp.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2xzofvqwe.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2zpfwpyyr.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2wpwigzyu.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2kiwfuupx.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2ydmxyhch.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2rznxcaqo.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2citqzfyv.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2opguggxa.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2bcwuhbyj.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2vmxsdcbc.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2elwyfkzm.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2dkxygbbs.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2adzuvguu.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2wmmkkklt.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2fjnurlxe.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2sgzvltgv.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2ramhgpsi.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2zcvekvkl.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2xhzaehie.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2rbzljvls.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2nrgtbigo.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2eaaaffsm.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2qaggesbo.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2ptpsacpg.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2zzwtnfdq.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2svaonmxu.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2dftzxewh.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2meqcmuce.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2qdrqqfxz.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2daippapy.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2gcptzogg.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2fzbnriqf.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2ncxpntmg.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2cvwpcbxa.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2ffzfjrmu.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2xupierve.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2upftsavz.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2ofxnoqyl.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2lnhqdouw.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2swcjxscn.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2cmueukcd.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2dwmivdql.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2lijmjnma.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2fwnbqwjk.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2zgkuepae.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2xsruvmst.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2yccqzltp.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2orpoxiuk.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2nbbnhvzt.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2fkpwiesk.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2akxmelwj.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2vrqmivss.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2bfvgatoi.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2zqpbackb.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2crsvllpu.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2hdxiepmp.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2widkavul.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2mrgcvxdg.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2mrhgprdh.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2kvfkwjvu.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2qsmpzefj.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2dudbgxno.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uhcrzhoo.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2qlhogzbe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2iyoomeut.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2xuyfhygr.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2ywytaxkw.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2aodynafj.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2lyytlunb.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2lfmxrmjn.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2fkhkcasu.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2wdbtoxra.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2egzqwdzq.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2lpbkistl.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2byhpleqg.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2mkivqeik.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2inpndkmb.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2iaydkegz.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2ylplhvne.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2bzqtpczy.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2woraupgt.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2dosmgdgo.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2lbzuobto.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2gccfkqwt.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2nlkpizrd.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2ekwktxzb.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2uboxbzvq.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2nenembsn.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ynfbzrbr.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2bwhahbmg.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2xvlyvkzg.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2gispwoek.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2jfbqbcji.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2cocmvdjb.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2giyebndw.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2papdnwnv.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2ikwnfayt.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2jsjmydmw.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2kxzuivrr.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2tcnrplcv.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2hxwndugz.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2lipuwstf.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2ubnfnzmx.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2qzopvsja.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2hrvdccff.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2efhvutho.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2hpjfgcwl.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2xobwzyyi.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2zimcsxwo.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2rrytjjhq.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2udrusfcl.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2wyjrgenx.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2oqlruujy.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2ubyecltd.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2hdimpasj.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2xlwfbyac.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2uxmukrdo.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2zatysaxf.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2raqebtvs.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2wifrjosa.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2txlxavuw.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2yhjnxikg.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2irjxexhf.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2rrzxdjod.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2zvowckpi.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2pxpqhwjn.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2rsvxcuru.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2tvpvtpgo.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2aynfezfu.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2kwjutwsa.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2hxtmzkim.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2fmzthhqu.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2toqfmjmi.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2wgjfrarj.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2axedvkob.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2aghummmq.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2iwdiutre.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2tqwworhe.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2dgxkridk.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2tilfqkgs.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2khqtcjgj.html


<!-- 参考信息 -->