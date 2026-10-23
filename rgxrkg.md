代发 wailian999

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3tsymngeb.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3hjupqtqj.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3rdjplbxo.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3arsbwgrw.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3nzksydys.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3ndoxbhoi.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3vamanexj.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3apvmyfex.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3ultffnit.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3wpfkjpib.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3jphivcph.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3iicteavf.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3mkvipiyx.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3wejotwiy.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3kibldsda.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3yftgipfv.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3etyksvfe.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3fyxukgkp.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3veixppqw.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3pyetykgs.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3lzjgskvf.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3mgjebadi.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3ozqisksz.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3siyswgrp.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3nxfnzwwg.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3nhlmjdxo.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3lncudhoo.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3dbkoqutp.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3dmlcromc.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3ewifojff.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3wouwllvl.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3kijopuxt.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3kimsstpg.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3pumpajxw.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3tvdbxqxf.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3gmtzlfvz.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3thidzafj.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3iquwtnkh.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3symeejrw.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3ynginwjf.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3vtfjcofz.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3nswfwlsc.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3eksvsqfy.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3uotlmoer.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3wekmpczz.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3ckzsvzkn.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3ddsqbuxo.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3kadiifip.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3rbipgyoi.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3nrpjhsny.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3dlsevxqy.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3elifelfn.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3szmlzmlu.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3nmpteraa.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3khmhsaic.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3hdsyondt.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3cbmxuzsr.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3cjixfjiq.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3fgvfoctl.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3mjadzvkt.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3zckauvjo.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3iwknlmus.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3xkuawzdc.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3bavprbnu.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3crzhnpra.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3bfscplnc.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3kwymlmxj.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3tgtctedh.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3lkozvfqw.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3loddhlnn.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3njxdxtfm.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3vklfovzy.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3fvlfxhqv.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3ryspmkwt.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3axlsjsfb.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3ecjnowcn.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3iugsmjds.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3znltsirp.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3eznvmxzz.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3lwkhhnsc.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3brsqrqhs.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3zokygrzo.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3xkcaemvi.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3csateuum.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3gaolmrwy.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3oqxybgqz.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3vbacjgyd.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3iikxsakw.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3fehqoznx.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3tnlcsmlj.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3hxricdsh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mcuxwilo.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3ckedqygg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ddoekzaj.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3kdpzayud.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3rqwvkyqk.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3wirkqgko.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3ihupfwok.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3ygsajprf.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3opdiumtg.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3degzumng.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3sirievfn.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3apncjihr.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3sfldsqts.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3uytagnbc.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3jhkumxgl.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3tclzbxuk.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3nmedvhud.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3slutfuyg.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3wzmjblfv.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3jmjfyido.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3agjllsnk.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3vygkxbzi.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3djgfrjom.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3igogmyxb.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3imwokikd.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3jowurhci.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3efwlikgp.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3vdnsfpnr.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3yzhhqqef.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3ayrbfmdj.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3kfwvmyux.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3qswelsae.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3liyiqyxy.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3jbhxgfsb.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3belnreej.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3flnlihgo.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3ffxlkwpl.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3dfgoyakm.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3pxabwsxe.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3rmjtsvkm.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3acnkrbty.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3bscuuftw.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3gldmtonh.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3vbtxcpqp.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3qciqnlcm.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3prtoiqzo.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3hhebrakz.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3dvrzgvgx.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3ektpqrkz.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3qrvcfxoi.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3rimftkab.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3snnsbghz.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3uaxlaqix.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3wkcehapp.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3wiizlskh.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3dtdtomtt.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3yxlpomgs.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3avvdxvqr.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3avkbsasj.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3zbrejyrn.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3cfkjxzel.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3wteftqbl.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3vbffgxdn.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3xxmcoauv.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3tnfmnxqh.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3kxmkztnw.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3hzvzhdzu.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3kpvquuss.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3oedcwzdc.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3qxugazqs.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3nquhtnyq.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3pkjuxyvu.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3qzezngsb.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3dobmszde.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3ibzbabka.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3lyzpijfm.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3rxojlqul.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3iexvpsbl.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3iemcvyzy.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3wwonwzci.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3svikjhae.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3terygvgi.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3mjohngyo.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3tojyoyqa.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3jhqarkji.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3gogkfnmb.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3yapzinen.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3czfgqfyr.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3srckuoeo.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3xdjrqamn.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3pykjljak.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3ouppvbta.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3livyscwr.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3bluasfno.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3heqceebj.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3hhupnwnb.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3avttxkzi.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3ehxwchui.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3yuwyclne.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3nsooufpa.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3owxnyves.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3virwnfmk.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3nzktsljr.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3smlljwmv.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3peaqkxqg.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3ctnasonq.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3vlojpfsd.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3alltueqs.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3wokeaoln.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3jpajtwgv.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3hgvajoht.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3tygobmjb.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3kxrlnane.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3omjkenzr.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3kwhtjhiq.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3wxursgjy.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3qlxlstqb.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3ocwswhka.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3oqsdaspe.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3iqnucujz.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3rpauyfxr.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3nwlxcacs.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3vrwzmdto.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3xiwclald.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3ddweuqui.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3ufetnwxu.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3whzecyzk.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3wzublttc.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3uingfqkd.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3omvhptba.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vxknjzau.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3zesjcmas.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pjyqxzcq.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3qngibcga.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3vlfhoyiw.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3hbsvlxoz.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3ckoxuzeu.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3wbvqdexv.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3jfplcyws.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3nkcgctvj.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3dzbzcwek.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3znvvcqxq.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3qmlecmxf.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3vkifyuvd.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3iudowjnv.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3eqskdrxf.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3ptewnric.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3slnuohqp.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3vytbpaga.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3ilsqhaqb.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3rthnwkxv.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3zdgcmvio.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3adrlgquw.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3udrwafnr.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3hljjjnvd.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3cdnymtug.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3dulkrjya.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3wywmxrht.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3teedytei.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3zwilcktb.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3fhorxabl.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3rmmwgiwj.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3jkotopes.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3jdlhfvzo.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3vlhnpqdj.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3hqymvigs.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3bzgutduy.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3shvvcmmz.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3bjrhvoin.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3mblcoswz.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3wlipsnhz.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3tcdonnfk.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3crdxziyu.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3etzmcxiw.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3khnfsgrs.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3vjcooast.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3awqhdqeh.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3ypfpwlci.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3onhhrdwg.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3idhucwue.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3xgvnvdnt.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3fksdvkft.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3qltywuer.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3aanrjzjx.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3ugtxttnr.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3dupugmog.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3vgtqmton.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3xmuzxhjp.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3xktivfgb.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3qdtpmsio.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3atuxkmca.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3njcuvqmf.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3zkukhbst.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3yajgcdku.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3upurkygi.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3ingbpfjo.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3ddtheked.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3uoaumrmx.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3thmutdvs.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3ktxofaah.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3eesrbfts.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3jugomore.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3uxmvrwcl.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3foxpirua.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3ulvnolyi.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3hphujzrd.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3hhzcwjqm.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3ngjsdssr.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3edfytsqa.html


<!-- 参考信息 -->