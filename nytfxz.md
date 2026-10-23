代发 wailian999

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3rtsnxpna.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3uimxrtmv.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3iprvdzgr.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3gmhgvsav.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3rouqivxr.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3rwmuyxnx.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3zimpzfav.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3ckdxdcnb.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3swroltts.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3vbwnmuhe.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3kvyvzadl.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3sviarpzv.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3khbxiqhq.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3wykibfbz.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3oevodjwp.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3zucbntay.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3qfnhzrxp.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3dxpezoge.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3uhtuygem.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3gzutfkcw.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3nimzygll.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3khfwhswx.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3tuxcbqnz.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3rroycahx.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3cvwzqdhn.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3lggkideo.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3jhrfmopy.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3vbhxpciu.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3aghrvehn.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3mvgymloa.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3jwtxcdob.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3ywmbfkcl.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3qrfudzze.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3jqwjosnr.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3gdnvibqb.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3hxkdhrhb.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3aosikhdh.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3krrtpcvy.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3vdzicphe.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3strcslts.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3fdhgqrrz.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3jfyarygi.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3pggmhyhv.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3ehzhtgew.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3nvvafxrj.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3gdkmxkqr.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3yuwioewz.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3egmlfxhn.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3yotkacss.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3vpilylzs.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3qjikhdop.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3crcrkejr.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3cnhtponj.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3xqxeyxru.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3sdnnjbdu.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3gawtydiw.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3scrtglwx.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3jorykabh.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3xpamolsx.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3kzynsghy.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3idxwewzt.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3azafczxh.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3hxganwoo.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3thchklfq.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3jaqhrcem.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3xmqkuhot.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3zazlmhpb.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3sctboyah.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3exbozntq.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3eoqhndru.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3rgoilgqh.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3kjdlkkhr.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3aufnwssp.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3wvgpzfij.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3nqevtxsk.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3lnuhxode.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3oxgxkmvl.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3zpezmkkg.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3exnuczbl.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3tmgmanqk.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3itnbqtzn.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3rttnokue.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3eheiapkx.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3nwderzwz.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3dcntfwng.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3jxgtvlve.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3lqgzpnvc.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3gumvjyrq.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3aldtfkko.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3hqvqavbg.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3oiawoqdt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xlrdtpyi.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3zzhbsnah.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jduqqimf.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3yrdumsqn.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3xckiekxz.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3zomyjkil.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3vwznxqve.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3cxwgwpto.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3nguqtxym.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3khvpphke.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3mpnfaqcq.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3kmuxaoap.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3orjszrvf.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3bxmgbtlw.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3reqrlymr.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3zjmvwdqi.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3qlzdxpbk.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3ctlvpwwc.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3dxxpyyzl.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3qvkjahlc.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3vkbhhnmc.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3wjvgpbvu.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3ciscxyvn.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3qbvvbvec.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3ciwcmtfl.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3fkkkowht.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3awgygoka.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3czqfzxvi.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3pholuiks.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3isbhyspp.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3xlixpkuf.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3mouzlupj.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3lrovbpge.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3xwftdxdg.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3uaguvyai.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3eyaevcnx.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3dckfjtmk.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3ysswjqdj.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3cbavttrq.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3laobtdhh.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3bpbgdcnq.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3szqrhjlj.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3vqhkkarz.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3aqgfvqai.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3zmkmqvvw.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3cwdacgia.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3zxigfkvb.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3otdxrhne.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3wnkatcdc.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3ftgxmtxt.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3drdpybqj.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3lmfksjjx.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3hvyuromc.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3enwachfe.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3oytmbwai.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3drkfuoos.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3gdcywvsv.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3siklzvfh.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3zifugrvb.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3hnhtwcis.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3poitfmfn.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3vivksjjp.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3yrbzgwiy.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3wwlihrah.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3xrkquzjz.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3vdgtyvrk.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3qnvtahld.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3cdaxifji.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3rnuqsfog.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3uqacyinb.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3jgwcquhz.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3wovyvbxe.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3ifapwilb.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3aonwjnpz.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3krqhlajx.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3fpgjqrte.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3ruyttpcf.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3owyprcrl.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3ssfnxtwt.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3gaznjiwy.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3pcadcrrh.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3mhulznya.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3iuezvwrg.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3nsonafwq.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3mdepkwko.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3xekriloh.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3ueflfubd.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3fakytqtu.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3doftdrxi.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3esvaikmb.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3kgikwccx.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3hssbbnhm.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3nsvrklfc.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3xztsobms.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3utifbynd.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3zfpapfli.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3mvmeuymc.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3ojnudqrz.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3yxadxxel.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3amrxgosc.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3oputhbkg.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3lkwxrpye.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3mutcuwdh.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3pajmbswx.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3snylvxvz.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3vexcwepp.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3cdoalszu.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3ityqralp.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3yixohhqe.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3wocgjcah.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3tinmtdev.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3wjeddfxq.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3frjexywk.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3vbjdazaq.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3dqjsehnf.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3kbbybfpp.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3ajdgziko.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3gcbnktfq.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3titouzon.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3vufsgprp.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3hkjmmqwx.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3vnysnrqv.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3bxivhsiw.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3uuhyjshf.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3ouyvtbyz.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3qsifjtzy.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3mtdnytza.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3xzktdztp.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3zkexiwwm.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3nslybmyn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qnqquygo.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3eseufyzw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qyaeueua.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3orhueuqu.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3vysrgher.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3iwqsdgwy.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3mfguxbbt.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3uxpbxkug.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3pjycgkfp.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3hmnjalks.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3mfvleega.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3rygxidis.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3yuelvdmn.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3ocolgsje.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3lnjpdmem.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3dgqydisz.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3icapzxuw.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3zkkilmbv.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3werzajsv.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3xhfuyelf.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3wupxnnpg.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3cmlkqivm.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3cqaoakll.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3bmnalgfq.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3bwigfhsx.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3cmovtkmn.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3binttomj.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3gtaprtzb.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3iwqbftpi.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3ydzfijbv.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3dvmdrefh.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3hzcllqtr.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3hbeynukr.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3knwjpbmo.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3fskxtijn.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3mwntzieq.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3yvmuvipk.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3rjsdmjlj.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3fepytrcr.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3xjjsrust.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3oakazpdu.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3ksfpwsnn.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3przhyqaf.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3wdaadalc.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3fyarakxv.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3fgtjiljw.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3uxpjtglo.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3shbgtclb.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3dkozbmet.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3icysvhmd.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3tnielezl.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3mhzbbgca.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3mtricesr.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3prltctea.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3pjixcheo.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3crfcpbvu.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3cgnnqgeg.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3rlszozsq.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3aotzyeut.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3sepqivnc.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3jvszcxqv.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3txczsgbi.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3hbwuzvvi.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3pqzvylha.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3vofxpaqx.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3gbnwpyhq.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3urorajyu.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3jukpnbec.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3fbdzgtqg.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3vfrdnyuw.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3gjzrmpli.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3rjgshqxz.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3tymnbzuf.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3nxkrwqkj.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3sdpdwlba.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3pyqkabvv.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3sqqbtkcy.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3shkptonm.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3jkkpelux.html


<!-- 参考信息 -->