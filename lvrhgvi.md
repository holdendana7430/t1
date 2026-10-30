代发 wailian999

cmd >/dev/null 2>&1
来源：http://wap.fanxiaobao.xyz/Article/details/ghwxoqeil.sHtML

[R42] 输入重定向
来源：http://baike.fanxiaobao.xyz/Article/details/gkhfwtowd.sHtML

wc -l < a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggamufeuw.sHtML

[R43] 按名字查找文件
来源：http://3g.fanxiaobao.xyz/Article/details/gpiheggcs.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geagnprae.sHtML

[R44] 按修改时间查找
来源：http://3g.fanxiaobao.xyz/Article/details/golrkgfgm.sHtML

find . -mtime -7 -type f
来源：http://mobile.fanxiaobao.xyz/Article/details/gackstdwm.sHtML

[R45] 批量删除
来源：http://baike.fanxiaobao.xyz/Article/details/gyyjacqsr.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.fanxiaobao.xyz/Article/details/glfgsmhvl.sHtML

[R46] 递归替换文件内容
来源：http://read.share.fanxiaobao.xyz/Article/details/gcyhypuje.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://m.share.fanxiaobao.xyz/Article/details/gttphyazg.sHtML

[R47] sed 单行替换
来源：http://read.share.fanxiaobao.xyz/Article/details/ghjjlgbmc.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/grdivvbnj.sHtML

[R48] awk 取指定列
来源：http://3g.fanxiaobao.xyz/Article/details/gaprrhdja.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gwqwkunha.sHtML

[R49] awk 带条件
来源：http://m.share.fanxiaobao.xyz/Article/details/gozsroolp.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.fanxiaobao.xyz/Article/details/gsoluqhhf.sHtML

[R50] awk 求和
来源：http://www.share.fanxiaobao.xyz/Article/details/gphykhygz.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gpobmrtes.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gekwwbair.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.fanxiaobao.xyz/Article/details/gmckukbxw.sHtML

[R52] 统计行数
来源：http://m.share.fanxiaobao.xyz/Article/details/gwdtnltih.sHtML

wc -l a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gcnidivvb.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.fanxiaobao.xyz/Article/details/gylrnicjv.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.fanxiaobao.xyz/Article/details/gvboojxea.sHtML

[R54] 比较两个文件
来源：http://3g.fanxiaobao.xyz/Article/details/gaawrsnjz.sHtML

diff a.txt b.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gqxpgvzuc.sHtML

[R55] 压缩与解压
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gountozdp.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.fanxiaobao.xyz/Article/details/gbmqnlcuv.sHtML

[R56] 远程拷贝
来源：http://read.share.fanxiaobao.xyz/Article/details/gfzrcsuas.sHtML

scp file user@host:/path/
来源：http://wap.fanxiaobao.xyz/Article/details/ghhmgeafa.sHtML

[R57] 远程执行命令
来源：http://wap.fanxiaobao.xyz/Article/details/gfiqrpawn.sHtML

ssh user@host 'uptime'
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggrbkczoo.sHtML

[R58] 下载文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/ganvouimj.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.fanxiaobao.xyz/Article/details/gjwjtstro.sHtML

[R59] 发 POST JSON
来源：http://read.share.fanxiaobao.xyz/Article/details/gkxnqwwih.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.fanxiaobao.xyz/Article/details/gentcpznp.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxdotzvgy.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.fanxiaobao.xyz/Article/details/gsxtgyddk.sHtML

[R61] 磁盘占用
来源：http://m.share.fanxiaobao.xyz/Article/details/gfgppayvo.sHtML

df -h;  du -sh *
来源：http://mobile.fanxiaobao.xyz/Article/details/gjastaloa.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gysujhuhj.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.fanxiaobao.xyz/Article/details/gxfoufytz.sHtML

[R63] 内存与进程
来源：http://baike.fanxiaobao.xyz/Article/details/gwjcudeop.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.fanxiaobao.xyz/Article/details/gdpveuzpd.sHtML

[R64] 结束进程
来源：http://blog.fanxiaobao.xyz/Article/details/gweofqyzw.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.fanxiaobao.xyz/Article/details/gaxxvifsv.sHtML

[R65] 查看端口占用
来源：http://3g.fanxiaobao.xyz/Article/details/gvestjoiy.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.fanxiaobao.xyz/Article/details/gckljkxlx.sHtML

[R66] 定时任务
来源：http://baike.fanxiaobao.xyz/Article/details/gzesljwfq.sHtML

crontab -e;  crontab -l
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsyrxldhq.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.fanxiaobao.xyz/Article/details/gehmaghdq.sHtML

openssl rand -hex 16
来源：http://m.share.fanxiaobao.xyz/Article/details/gwetgaguu.sHtML

[R68] 计算文件校验值
来源：http://3g.fanxiaobao.xyz/Article/details/gtjqsdvnf.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gimsqwnbt.sHtML

[R69] 生成随机密码
来源：http://wap.fanxiaobao.xyz/Article/details/gynhfgxkl.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.fanxiaobao.xyz/Article/details/ghzykvent.sHtML

[R70] 时间戳与互转
来源：http://mobile.fanxiaobao.xyz/Article/details/gmwbrkrci.sHtML

date +%s;  date -d @1700000000
来源：http://3g.fanxiaobao.xyz/Article/details/giukvyuew.sHtML

[R71] 日期格式化
来源：http://read.share.fanxiaobao.xyz/Article/details/giyzioufk.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://read.share.fanxiaobao.xyz/Article/details/gjenjefnj.sHtML

[R72] 等待端口就绪
来源：http://3g.fanxiaobao.xyz/Article/details/gtfdgdtmc.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gfvjygjln.sHtML

[R73] 分割大日志
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmjccupvq.sHtML

split -l 1000 big.log part_
来源：http://read.share.fanxiaobao.xyz/Article/details/gaqowgueo.sHtML

[R74] 批量重命名
来源：http://m.share.fanxiaobao.xyz/Article/details/gnvbyytct.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.fanxiaobao.xyz/Article/details/gjpcbtyed.sHtML

[R75] 导出环境变量
来源：http://baike.fanxiaobao.xyz/Article/details/gcfpagsoo.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.fanxiaobao.xyz/Article/details/gqkvzhyaq.sHtML

[R76] 使用临时文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcmyqdwjs.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fanxiaobao.xyz/Article/details/guqgnqqdv.sHtML

[R77] 读取用户输入
来源：http://baike.fanxiaobao.xyz/Article/details/gultxzmtp.sHtML

read -rp "请输入: " ans
来源：http://mobile.fanxiaobao.xyz/Article/details/ghoikcgxj.sHtML

[R78] 交互式菜单
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glbbtajbh.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzdjqpfdp.sHtML

[R79] 解析命令行选项
来源：http://3g.fanxiaobao.xyz/Article/details/gdhmuhkfs.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.fanxiaobao.xyz/Article/details/ghaezynzz.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.fanxiaobao.xyz/Article/details/gjaebdolu.sHtML

time ./run.sh
来源：http://www.share.fanxiaobao.xyz/Article/details/guzpamczy.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gjdmuqscm.sHtML

S. C / C++ 专题
来源：http://read.share.fanxiaobao.xyz/Article/details/gpwfgrrtx.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gojdddcar.sHtML

[S01] C：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gwanbaupr.sHtML

#include <stdio.h>
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gghxokaib.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gkcectokt.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqwvoljft.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.fanxiaobao.xyz/Article/details/gmiynklci.sHtML

[S03] C：读入整数
来源：http://mobile.fanxiaobao.xyz/Article/details/gukyjoqqj.sHtML

int x; scanf("%d", &x);
来源：http://baike.fanxiaobao.xyz/Article/details/gymymngtb.sHtML

[S04] C：字符串复制
来源：http://blog.fanxiaobao.xyz/Article/details/gmcwzmbvm.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.fanxiaobao.xyz/Article/details/gujzzmlmd.sHtML

[S05] C：字符串长度
来源：http://3g.fanxiaobao.xyz/Article/details/gpxrmqmqy.sHtML

strlen(s)
来源：http://m.share.fanxiaobao.xyz/Article/details/gmanovuuo.sHtML

[S06] C：字符串比较
来源：http://wap.fanxiaobao.xyz/Article/details/gprzerjdx.sHtML

strcmp(a, b) == 0
来源：http://mobile.fanxiaobao.xyz/Article/details/gczrhvrrr.sHtML

[S07] C：数组遍历求和
来源：http://3g.fanxiaobao.xyz/Article/details/gvdqmarkc.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.fanxiaobao.xyz/Article/details/gyxbrjxik.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.fanxiaobao.xyz/Article/details/gkhsiallx.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxadnbbct.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.fanxiaobao.xyz/Article/details/gotlpcpqa.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.fanxiaobao.xyz/Article/details/gwntypeoc.sHtML

[S10] C：指针与解引用
来源：http://m.share.fanxiaobao.xyz/Article/details/gbmiaqxcz.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.fanxiaobao.xyz/Article/details/gwuxmnogl.sHtML

[S11] C：逐行读文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gjpqfwdcb.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.fanxiaobao.xyz/Article/details/gnagmibxc.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.fanxiaobao.xyz/Article/details/gcqjhmals.sHtML

fclose(f);
来源：http://www.share.fanxiaobao.xyz/Article/details/geqvkkscg.sHtML

[S12] C：写文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gvaulnfes.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.fanxiaobao.xyz/Article/details/gegydhtge.sHtML

[S13] C：宏定义
来源：http://www.share.fanxiaobao.xyz/Article/details/gfwqhmvpv.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.fanxiaobao.xyz/Article/details/gtyjysbvx.sHtML

[S14] C：枚举
来源：http://www.share.fanxiaobao.xyz/Article/details/gjoivxryd.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.fanxiaobao.xyz/Article/details/gsynrpkno.sHtML

[S15] C：类型转换
来源：http://3g.fanxiaobao.xyz/Article/details/glashonpy.sHtML

(double) a / b
来源：http://mobile.fanxiaobao.xyz/Article/details/gkvkzaazn.sHtML

[S16] C：位操作置位
来源：http://mobile.fanxiaobao.xyz/Article/details/ggxxmdkiv.sHtML

x |= (1 << 3);
来源：http://mobile.fanxiaobao.xyz/Article/details/gzprbmwwo.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.fanxiaobao.xyz/Article/details/gokltoqjx.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.fanxiaobao.xyz/Article/details/gjwlqhvwq.sHtML

[S18] C：命令行参数
来源：http://www.share.fanxiaobao.xyz/Article/details/gvtlsxthl.sHtML

int main(int argc, char **argv)
来源：http://3g.fanxiaobao.xyz/Article/details/gleelcige.sHtML

[S19] C：快速排序
来源：http://baike.fanxiaobao.xyz/Article/details/grmbqklqo.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.fanxiaobao.xyz/Article/details/guuqoiypu.sHtML

[S20] C：二分查找
来源：http://mobile.fanxiaobao.xyz/Article/details/gggelvpdy.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grmuwimen.sHtML

[S21] C：字符类别判断
来源：http://blog.fanxiaobao.xyz/Article/details/gixxuihqd.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.fanxiaobao.xyz/Article/details/gfoesqmpq.sHtML

[S22] C：字符串转数字
来源：http://www.blog.fanxiaobao.xyz/Article/details/gywdduvhx.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.fanxiaobao.xyz/Article/details/gprknfwqp.sHtML

[S23] C：随机数
来源：http://www.share.fanxiaobao.xyz/Article/details/goejjbxjb.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.fanxiaobao.xyz/Article/details/gejbojtkl.sHtML

[S24] C：获取本地时间
来源：http://3g.fanxiaobao.xyz/Article/details/gwyuauccd.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.fanxiaobao.xyz/Article/details/ggkqhdexe.sHtML

[S25] C：内存拷贝
来源：http://blog.fanxiaobao.xyz/Article/details/gzpafefdj.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqyzheast.sHtML

[S26] C：内存清零
来源：http://blog.fanxiaobao.xyz/Article/details/gpequcirw.sHtML

memset(a, 0, sizeof a);
来源：http://blog.fanxiaobao.xyz/Article/details/gzrwfyuph.sHtML

[S27] C：定义常量
来源：http://read.share.fanxiaobao.xyz/Article/details/gcubjrewm.sHtML

const double PI = 3.14159;
来源：http://mobile.fanxiaobao.xyz/Article/details/gdxiabisa.sHtML

[S28] C：静态变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkzqfuwzi.sHtML

static int counter = 0;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcbgtcvep.sHtML

[S29] C：变参函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvasxirax.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.fanxiaobao.xyz/Article/details/gcuesenty.sHtML

[S30] C：头文件保护
来源：http://www.share.fanxiaobao.xyz/Article/details/gtajgvfqd.sHtML

#ifndef X_H
来源：http://read.share.fanxiaobao.xyz/Article/details/gpoqxwfnj.sHtML

#define X_H
来源：http://www.share.fanxiaobao.xyz/Article/details/ggxraxzwi.sHtML

#endif
来源：http://wap.fanxiaobao.xyz/Article/details/goahwsoao.sHtML

[S31] C++：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gfjmovtqw.sHtML

#include <iostream>
来源：http://read.share.fanxiaobao.xyz/Article/details/ggjqdujet.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.fanxiaobao.xyz/Article/details/gkirbxoot.sHtML

[S32] C++：字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/gckrnpuwi.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.fanxiaobao.xyz/Article/details/gvudtusbh.sHtML

[S33] C++：vector 增删
来源：http://read.share.fanxiaobao.xyz/Article/details/gocsmeror.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.fanxiaobao.xyz/Article/details/gnvpuppiy.sHtML

[S34] C++：遍历 vector
来源：http://read.share.fanxiaobao.xyz/Article/details/gvcsrfyyk.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.fanxiaobao.xyz/Article/details/ggrvxpakj.sHtML

[S35] C++：map
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxrudoggh.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fanxiaobao.xyz/Article/details/gwhdsawxe.sHtML

[S36] C++：unordered_map
来源：http://mobile.fanxiaobao.xyz/Article/details/gwcgodqta.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fanxiaobao.xyz/Article/details/gxdmxymfw.sHtML

[S37] C++：set
来源：http://www.blog.fanxiaobao.xyz/Article/details/guyvaajsk.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.fanxiaobao.xyz/Article/details/gbscvxcvy.sHtML

[S38] C++：排序
来源：http://blog.fanxiaobao.xyz/Article/details/gflwpenwi.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.fanxiaobao.xyz/Article/details/gjviqckpq.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsuyytclq.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfcfzwfzk.sHtML

[S40] C++：查找元素
来源：http://read.share.fanxiaobao.xyz/Article/details/gbkkagvgj.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gktqqfnea.sHtML

[S41] C++：类与构造函数
来源：http://blog.fanxiaobao.xyz/Article/details/gdffqaxpu.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.fanxiaobao.xyz/Article/details/gfxvxlkdr.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghvkstdoi.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.fanxiaobao.xyz/Article/details/gzaagyixh.sHtML

[S43] C++：智能指针
来源：http://baike.fanxiaobao.xyz/Article/details/ghiqvzkff.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.fanxiaobao.xyz/Article/details/gkcvaxjjl.sHtML

[S44] C++：引用传参
来源：http://wap.fanxiaobao.xyz/Article/details/gaqdpqzez.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gapjsbolo.sHtML

[S45] C++：lambda
来源：http://www.share.fanxiaobao.xyz/Article/details/gqypkctkq.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkqsezyum.sHtML

[S46] C++：函数模板
来源：http://www.share.fanxiaobao.xyz/Article/details/gcjdjyyqe.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.fanxiaobao.xyz/Article/details/gbrphgkyy.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.fanxiaobao.xyz/Article/details/gyqzsjhbu.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gpzokikmv.sHtML

[S48] C++：逐行读文件
来源：http://blog.fanxiaobao.xyz/Article/details/gxpfnnnxz.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzpfymahy.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.fanxiaobao.xyz/Article/details/gwclealdh.sHtML

[S49] C++：写文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/goaychkpp.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.fanxiaobao.xyz/Article/details/gwckvujad.sHtML

[S50] C++：格式化数字
来源：http://www.share.fanxiaobao.xyz/Article/details/ghzimypun.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.fanxiaobao.xyz/Article/details/glvyycqft.sHtML

[S51] C++：显式类型转换
来源：http://m.share.fanxiaobao.xyz/Article/details/guodpwkvt.sHtML

static_cast<double>(a) / b
来源：http://mobile.fanxiaobao.xyz/Article/details/gemrqttmd.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.fanxiaobao.xyz/Article/details/gphqdgzxl.sHtML

int size() const noexcept { return n_; }
来源：http://blog.fanxiaobao.xyz/Article/details/goudckvnj.sHtML

[S53] C++：移动语义
来源：http://m.share.fanxiaobao.xyz/Article/details/gfcvwtgtn.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.fanxiaobao.xyz/Article/details/gawzgfyvd.sHtML

[S54] C++：异常处理
来源：http://wap.fanxiaobao.xyz/Article/details/gfqyxbhud.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.fanxiaobao.xyz/Article/details/gsolfbekn.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtcbqglkz.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gygxfnsil.sHtML

[S56] C++：optional
来源：http://mobile.fanxiaobao.xyz/Article/details/gkayfwwav.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.fanxiaobao.xyz/Article/details/gsntjalua.sHtML

[S57] C++：编译期常量
来源：http://3g.fanxiaobao.xyz/Article/details/gvtruhpnt.sHtML

constexpr int N = 10;
来源：http://mobile.fanxiaobao.xyz/Article/details/gosqyyemz.sHtML

[S58] C++：命名空间
来源：http://read.share.fanxiaobao.xyz/Article/details/gftcdahdr.sHtML

namespace ns { int f() { return 1; } }
来源：http://blog.fanxiaobao.xyz/Article/details/gkkhcseqb.sHtML

[S59] C++：静态断言
来源：http://www.share.fanxiaobao.xyz/Article/details/ghswizbpt.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.fanxiaobao.xyz/Article/details/gkzirvpnb.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.fanxiaobao.xyz/Article/details/gigfvcdnh.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.fanxiaobao.xyz/Article/details/gkgifwyem.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gxvshjwoi.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.fanxiaobao.xyz/Article/details/gbbosctij.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gezbassng.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwvdnjcwi.sHtML

println("Hello")
来源：http://baike.fanxiaobao.xyz/Article/details/gcxzhside.sHtML

[T02] Kotlin：变量
来源：http://3g.fanxiaobao.xyz/Article/details/gsqpupmak.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.fanxiaobao.xyz/Article/details/gqorzpssg.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.fanxiaobao.xyz/Article/details/gshfcizvl.sHtML

"值: $b"
来源：http://3g.fanxiaobao.xyz/Article/details/gqmrfslxu.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpnlafcmy.sHtML

val n: String? = null;  n?.length
来源：http://m.share.fanxiaobao.xyz/Article/details/gdzstgkkt.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.fanxiaobao.xyz/Article/details/gnzaydfhl.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.fanxiaobao.xyz/Article/details/gujffxygq.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.fanxiaobao.xyz/Article/details/gfeckcazj.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.fanxiaobao.xyz/Article/details/girlxrgpq.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.fanxiaobao.xyz/Article/details/gnbrvicsq.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.fanxiaobao.xyz/Article/details/gootauskj.sHtML

[T08] Kotlin：数据类
来源：http://3g.fanxiaobao.xyz/Article/details/gihjwjscy.sHtML

data class User(val name: String, val age: Int)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzlmsgdpq.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.fanxiaobao.xyz/Article/details/gpsxueyih.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.fanxiaobao.xyz/Article/details/gxapupode.sHtML

[T10] Kotlin：默认参数
来源：http://wap.fanxiaobao.xyz/Article/details/gcmcvzljy.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.fanxiaobao.xyz/Article/details/grzubzuix.sHtML

[T11] Kotlin：协程
来源：http://baike.fanxiaobao.xyz/Article/details/gcuwvhdfc.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://blog.fanxiaobao.xyz/Article/details/gfcqahgyu.sHtML

[T12] Kotlin：解构声明
来源：http://blog.fanxiaobao.xyz/Article/details/gpndhxidj.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.fanxiaobao.xyz/Article/details/gwmehorxw.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.fanxiaobao.xyz/Article/details/gepmzmabp.sHtML

val m = mapOf("a" to 1)
来源：http://baike.fanxiaobao.xyz/Article/details/gaeacxywu.sHtML

[T14] Kotlin：循环
来源：http://wap.fanxiaobao.xyz/Article/details/glfbtnuhb.sHtML

for (i in 1..10) println(i)
来源：http://read.share.fanxiaobao.xyz/Article/details/gdugffnsx.sHtML

[T15] Kotlin：接口
来源：http://read.share.fanxiaobao.xyz/Article/details/glwvmjokv.sHtML

interface Shape { fun area(): Double }
来源：http://m.share.fanxiaobao.xyz/Article/details/gfcraukmj.sHtML

[T16] Swift：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gcznooxei.sHtML

print("Hello")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gweknznpc.sHtML

[T17] Swift：变量与常量
来源：http://wap.fanxiaobao.xyz/Article/details/gdkgpafjs.sHtML

var a = 1;  let b = 2
来源：http://wap.fanxiaobao.xyz/Article/details/gntmfajzs.sHtML

[T18] Swift：字符串插值
来源：http://mobile.fanxiaobao.xyz/Article/details/gzdbpljxb.sHtML

"值: \(b)"
来源：http://baike.fanxiaobao.xyz/Article/details/gvhqokygk.sHtML

[T19] Swift：可选绑定
来源：http://blog.fanxiaobao.xyz/Article/details/glxdburmy.sHtML

if let n = opt { print(n) }
来源：http://read.share.fanxiaobao.xyz/Article/details/gsbnwgyrn.sHtML

[T20] Swift：数组操作
来源：http://3g.fanxiaobao.xyz/Article/details/gvuvesobq.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://baike.fanxiaobao.xyz/Article/details/goifuftab.sHtML

[T21] Swift：遍历
来源：http://wap.fanxiaobao.xyz/Article/details/getprszmv.sHtML

for x in a { print(x) }
来源：http://baike.fanxiaobao.xyz/Article/details/goikhakse.sHtML

[T22] Swift：字典
来源：http://mobile.fanxiaobao.xyz/Article/details/gbgoecngf.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://3g.fanxiaobao.xyz/Article/details/gkjhnyxlo.sHtML

[T23] Swift：函数
来源：http://wap.fanxiaobao.xyz/Article/details/gkcfoybar.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.share.fanxiaobao.xyz/Article/details/guafqgktf.sHtML

[T24] Swift：闭包
来源：http://read.share.fanxiaobao.xyz/Article/details/gywxqrvln.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvzsyjaot.sHtML

[T25] Swift：结构体
来源：http://read.share.fanxiaobao.xyz/Article/details/gsbkryhap.sHtML

struct P { var x: Int }
来源：http://blog.fanxiaobao.xyz/Article/details/gensijdqm.sHtML

[T26] Swift：类与重写
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjdhjybbl.sHtML

class A: Base { override func f() {} }
来源：http://blog.fanxiaobao.xyz/Article/details/gsuzwgpbu.sHtML

[T27] Swift：错误处理
来源：http://wap.fanxiaobao.xyz/Article/details/gvewnqfjp.sHtML

do { try f() } catch { print(error) }
来源：http://blog.fanxiaobao.xyz/Article/details/goicvlmci.sHtML

[T28] Swift：枚举
来源：http://baike.fanxiaobao.xyz/Article/details/govvsiscb.sHtML

enum Color { case red, green }
来源：http://wap.fanxiaobao.xyz/Article/details/geshapgxq.sHtML

[T29] Swift：guard 提前返回
来源：http://www.blog.fanxiaobao.xyz/Article/details/granstgpy.sHtML

guard let x = opt else { return }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqrcgxsjq.sHtML

[T30] Swift：协议
来源：http://mobile.fanxiaobao.xyz/Article/details/gnrypllzd.sHtML

protocol Shape { func area() -> Double }
来源：http://blog.fanxiaobao.xyz/Article/details/gxcpnxahb.sHtML

[T31] Lua：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gavkngcfl.sHtML

print("Hello")
来源：http://baike.fanxiaobao.xyz/Article/details/geeohsplg.sHtML

[T32] Lua：局部变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gdbofwauz.sHtML

local a = 1
来源：http://m.share.fanxiaobao.xyz/Article/details/glqkgmohp.sHtML

[T33] Lua：表（数组）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjphrvtsx.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://baike.fanxiaobao.xyz/Article/details/gqrkxapxf.sHtML

[T34] Lua：遍历表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glcaduejs.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://baike.fanxiaobao.xyz/Article/details/ghpgwhrfc.sHtML

[T35] Lua：字典表
来源：http://wap.fanxiaobao.xyz/Article/details/givdsjfaj.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.share.fanxiaobao.xyz/Article/details/glfaodocq.sHtML

[T36] Lua：函数
来源：http://3g.fanxiaobao.xyz/Article/details/gsguhvnbf.sHtML

function add(a, b) return a + b end
来源：http://3g.fanxiaobao.xyz/Article/details/gpodwggjx.sHtML

[T37] Lua：字符串拼接
来源：http://www.blog.fanxiaobao.xyz/Article/details/gspaxmfeh.sHtML

"a" .. "b"
来源：http://blog.fanxiaobao.xyz/Article/details/gorhvyhrp.sHtML

[T38] Lua：条件
来源：http://read.share.fanxiaobao.xyz/Article/details/gzkxkhcco.sHtML

if x > 0 then print("正") end
来源：http://mobile.fanxiaobao.xyz/Article/details/gvhymdiet.sHtML

[T39] Lua：模式匹配
来源：http://blog.fanxiaobao.xyz/Article/details/gkehjydcm.sHtML

string.find(s, "%d+")
来源：http://wap.fanxiaobao.xyz/Article/details/gvtestoci.sHtML

[T40] Lua：元表
来源：http://m.share.fanxiaobao.xyz/Article/details/gavrqtgtq.sHtML

setmetatable({}, { __index = base })
来源：http://m.share.fanxiaobao.xyz/Article/details/gcrwohrug.sHtML

[T41] Perl：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyoudfwrn.sHtML

print "Hello\n";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqecnzheq.sHtML

[T42] Perl：变量类型
来源：http://www.share.fanxiaobao.xyz/Article/details/getuqsqzf.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://baike.fanxiaobao.xyz/Article/details/gjbdkgzcq.sHtML

[T43] Perl：字符串插值
来源：http://wap.fanxiaobao.xyz/Article/details/gsykjdykp.sHtML

"值: $a"
来源：http://read.share.fanxiaobao.xyz/Article/details/gvvpggqbl.sHtML

[T44] Perl：条件
来源：http://blog.fanxiaobao.xyz/Article/details/grbaiuyih.sHtML

if ($a > 0) { print "正"; }
来源：http://wap.fanxiaobao.xyz/Article/details/gcshidkby.sHtML


<!-- 参考信息 -->