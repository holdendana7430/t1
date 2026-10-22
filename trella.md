代发 wailian999

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2jkhefvta.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2ktqemfia.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2mqdtwvrj.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2ypzilmaq.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2pzelqogm.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2bzzfquyn.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2bilfheqw.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2bmzjpiza.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2uxlbvgef.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2odvkijdt.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2ghvifnrw.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2zcviwggn.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2glgsiihq.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2qmjvkuet.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2fyklxzey.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2cfoljdsm.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2qhlzmlml.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2sexqhbvy.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2nexgscpu.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2hjkckttf.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2qzdjvbog.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2qwtefxom.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2uvacdgjp.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2cbqilfme.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2wbrmhnkk.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2lavewuxy.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2hkovzljw.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2kbacware.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2uzwctzmw.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2txkqozhk.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2exsqbbtk.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2eorsvalk.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2fshlvrrt.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2wjqahxkj.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2koirlsvz.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2nkydwhtg.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2kyqonxid.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2zxnfeoxo.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2frrrzzae.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2xjivapht.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2qgxtvzmc.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2fzloepyq.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2jnhmrwel.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2cbxpgofu.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2maqsobxg.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2cextitmi.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2cuttycyg.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2vjnhucvp.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2stbndfwv.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2nfzqhtbr.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2yjiaizlw.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2ogwiajio.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2sgkblxdk.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2ocejdpol.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2xzknfrbo.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2vywvytoy.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2mwlalzic.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2ibbpjfsl.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2kvpdlnky.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2nvueknth.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2zsmraiex.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2nlrjhway.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2wkywjvss.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2jbjwgawk.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2gbichfty.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2emjciznv.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2ngvckkry.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2qvvutjxe.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2knouznow.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2ihczmhob.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2qiwvfuvh.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2uvzmzrcb.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2uoqyaxoq.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2ifwutsub.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2witahyef.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2noztzhjf.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2spifmzbu.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2zemkdymg.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2eztfdase.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2hfcdyxjg.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2edxbduem.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2lswjetun.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2uykodzel.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2umihtljg.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2tbrefloz.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2eykjfpss.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2hukbhxvz.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2ktirgrxh.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2udlwgzgf.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2zxvmqdzc.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2pskjlivq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vnljnegs.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2onwaqwds.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uktwurfr.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2xyenoiyy.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2rpbgtprs.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2pxlrzwcs.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2vehybocc.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2aabgoyyq.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2ohptcqro.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2yxaqmwkk.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2arvclvbj.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2toafvdtr.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2rzwnlouo.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2efcqvrsg.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2dpekureb.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2yloxtgcf.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2qbvjriac.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2txumbzbx.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2uysfudfx.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2zxppmvhu.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2eiawaukk.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2ytwthrjg.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2rwgcdyyy.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2sihqgtvi.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2cabujeij.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2cvtrrong.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2qwrlsaph.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2cumcrvzt.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2sfslfqns.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2klhqpvjc.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2grteokne.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2oomftist.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2zixmbyxt.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2qjjseewj.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2ieveahmg.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2jzmovrip.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2wbmrhcch.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2caabyteb.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2epnzosiu.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2jigcxspd.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2cbbpurgw.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2kkjdgwtd.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2wdetcfqg.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2azjfvgbv.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2mgnktkwo.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2iinlpfef.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2jpqfugna.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2kvvphhpy.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2flrgcjkm.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2qomkkgfz.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2iuekqolc.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2qpqixzxo.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2mxmenefc.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2azqszqbg.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2rizsrpby.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2pxvxtksi.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2nxqabpcj.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2jyqkukam.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2sqbnrzil.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2pcyswbch.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2wmlkiizj.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2dbshtnqe.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2txqkfuct.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2tyiqdqmi.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2wuyzsfjf.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2uymukihc.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2rlzkgnhe.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2ajrsjqgb.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2jdajtxlq.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2jdohegtl.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2mdhkwyjr.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2yrpvzfvw.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2mvevtmxd.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2xganplon.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2ktfjszfl.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2zmvdgnaw.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2xeeyzgsn.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2cxjusumx.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2cfwgmiqx.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2spskknlm.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2oznmqzat.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2iiuorkzv.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2ieswpooy.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2pzzzapqh.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2vfufiuim.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2izwnrrdd.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2yzfzwhfe.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2umjwmnkc.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2yqkrxbat.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2nqmnqmhx.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2aporgooe.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2ugtsgtzo.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2qvaltkae.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2xdygvnma.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2vexzrarm.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2twbsjfbn.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2ldtzkiey.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2kjkpcyvb.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2mqxkngrm.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2eradjmfw.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2kyhlfnxj.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2gqphlhgl.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2pypkwgjc.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2vdpvzgez.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2akjrlmfg.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2gzvdodbj.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2mgswxypf.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2hukkpamr.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2yczjbgos.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2ewuwbged.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2ekxjynwu.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2pgodeeqp.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2zzyhtyex.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2jfpqsbmn.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2tqtmdeqj.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2nbxqemdb.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2qllydtkr.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2qblvziok.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2bwvcbvxe.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2tocrflgg.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2glkglqnc.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2wbryrjvz.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2ohyfprwe.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2veyapfxf.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2oqkjbtrt.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2mwtvzplt.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2femohdvo.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2rloqapuv.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2vjwkjcji.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2rwcapkng.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2oedwxgun.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2pejhwoas.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jmovzjkn.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ehmlrwyi.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2mrbdaiwc.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2tztvppaq.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2koeocnpu.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2wnbwyssx.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2ahucviqf.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2qcrcnbob.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2aulauwcp.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2wzpjeuec.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2hoxbfqhp.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2wjgdvjhl.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2sesyrjez.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2qezcaaxs.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2skejlpai.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2bciqpsnb.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2twomlsvg.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2ovtmcqaw.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2zziwgcgd.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2szdwqinv.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2ozykgbsj.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2teielgtd.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2ikosgmnr.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2lpizpaxs.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2pfgzfvot.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2ofabvftf.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2budyfkch.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2mgjketel.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2yltkvfdb.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2pwxmoafy.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2bcjtxsud.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2qttcnboe.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2zhgysosi.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2rwqwdhkp.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2zlyuxprb.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2fcxklcvj.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2rvfqcfok.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2hfxppzac.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2lwsevjru.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2bsbsogdt.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2dmlnjwkp.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2xvhkfoek.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2tkmzdfxp.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2etjgextn.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2vhbqskqb.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2mthasfua.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2jwmwjkzf.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2yvtnbyom.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2tapdrdmf.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2xewntmhs.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2wexabyqm.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2qhouufbf.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2tnfpwbxm.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2ogpysuob.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2kzerqhhz.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2spciolxt.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2drbqzqgw.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2itdxdhrz.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2fvsimnws.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2etolcqwj.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2npiusgxg.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2kbyfvmog.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2ejtiswog.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2asbbdftx.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2wudyffnz.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2urnrnrco.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2nufplsbm.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2kpwmnkzp.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2swkkzhwj.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2ecaqnxgf.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2prdtbqls.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2lojzwpto.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2sgxdjjvv.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2uqgcdvkh.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2pchsbfwk.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2ttomnaeq.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2ngzvdvsn.html


<!-- 参考信息 -->