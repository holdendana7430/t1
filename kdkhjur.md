代发 wailian999

sleep 5 & pid=$!; wait "$pid"
来源：http://3g.zdbjq.cn/Article/details/gkgwwekjx.sHtML

[R36] 并发执行多个任务
来源：http://baike.hesvh.cn/Article/details/gjbgruohq.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.fehbvm.com/Article/details/gnayfmvaf.sHtML

[R37] 把输出赋给变量
来源：http://baike.fehbvm.com/Article/details/grukoqtil.sHtML

files=$(ls -1)
来源：http://blog.fehbvm.com/Article/details/grhfgrykh.sHtML

[R38] 管道串联
来源：http://www.m.share.hesvh.cn/Article/details/gcwwxpzfg.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.hesvh.cn/Article/details/giiatkukg.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.zdbjq.cn/Article/details/gwyxntsyu.sHtML

cmd > out.log 2>&1
来源：http://www.blog.zdbjq.cn/Article/details/gvsbsmham.sHtML

[R40] 追加写日志
来源：http://3g.fehbvm.com/Article/details/ganmtvkqh.sHtML

echo "log" >> out.log
来源：http://www.share.fehbvm.com/Article/details/gmtbhxkdz.sHtML

[R41] 丢弃输出
来源：http://read.share.fehbvm.com/Article/details/gbuhoejgt.sHtML

cmd >/dev/null 2>&1
来源：http://3g.zdbjq.cn/Article/details/gvhitlefh.sHtML

[R42] 输入重定向
来源：http://m.share.hesvh.cn/Article/details/gqizsrqqx.sHtML

wc -l < a.txt
来源：http://baike.fehbvm.com/Article/details/graxrrctk.sHtML

[R43] 按名字查找文件
来源：http://www.blog.zdbjq.cn/Article/details/gxlnaqqzs.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.hesvh.cn/Article/details/gzmlljexj.sHtML

[R44] 按修改时间查找
来源：http://read.share.hesvh.cn/Article/details/gpshjtfnn.sHtML

find . -mtime -7 -type f
来源：http://www.share.zdbjq.cn/Article/details/gcykebjle.sHtML

[R45] 批量删除
来源：http://wap.fehbvm.com/Article/details/gzdkupeje.sHtML

find . -name "*.tmp" -delete
来源：http://3g.fehbvm.com/Article/details/gkzsalbdd.sHtML

[R46] 递归替换文件内容
来源：http://read.share.zdbjq.cn/Article/details/gnsldumdl.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.fehbvm.com/Article/details/guqtzurij.sHtML

[R47] sed 单行替换
来源：http://www.share.fehbvm.com/Article/details/geszpmeuw.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.zdbjq.cn/Article/details/gjrkcjrfk.sHtML

[R48] awk 取指定列
来源：http://3g.hesvh.cn/Article/details/gsrqkknqj.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.fehbvm.com/Article/details/gsaeajgpb.sHtML

[R49] awk 带条件
来源：http://read.share.hesvh.cn/Article/details/gvkolythw.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.zdbjq.cn/Article/details/gsgrgmybc.sHtML

[R50] awk 求和
来源：http://mobile.hesvh.cn/Article/details/gwfrorbgk.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.zdbjq.cn/Article/details/gsoyqecos.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.zdbjq.cn/Article/details/gxhbgtfvn.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.zdbjq.cn/Article/details/goiwvrmrm.sHtML

[R52] 统计行数
来源：http://www.m.share.zdbjq.cn/Article/details/gaafcncbc.sHtML

wc -l a.txt
来源：http://wap.fehbvm.com/Article/details/gmpllzyek.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.hesvh.cn/Article/details/gfevsofkg.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.fehbvm.com/Article/details/gwlhzphlo.sHtML

[R54] 比较两个文件
来源：http://www.m.share.hesvh.cn/Article/details/gmhurvorn.sHtML

diff a.txt b.txt
来源：http://blog.zdbjq.cn/Article/details/glhxyeswe.sHtML

[R55] 压缩与解压
来源：http://m.share.fehbvm.com/Article/details/gzyswwjkz.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.hesvh.cn/Article/details/gltbodmkb.sHtML

[R56] 远程拷贝
来源：http://blog.zdbjq.cn/Article/details/gecowiftq.sHtML

scp file user@host:/path/
来源：http://mobile.fehbvm.com/Article/details/ggkmmzljk.sHtML

[R57] 远程执行命令
来源：http://wap.zdbjq.cn/Article/details/gagygolry.sHtML

ssh user@host 'uptime'
来源：http://www.blog.zdbjq.cn/Article/details/guulzcvcj.sHtML

[R58] 下载文件
来源：http://mobile.zdbjq.cn/Article/details/gwuusafpe.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.zdbjq.cn/Article/details/gjacizqwq.sHtML

[R59] 发 POST JSON
来源：http://read.share.zdbjq.cn/Article/details/gupsozpze.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.hesvh.cn/Article/details/gvcfzsepu.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.fehbvm.com/Article/details/gqyarnnsw.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.fehbvm.com/Article/details/gwraaeido.sHtML

[R61] 磁盘占用
来源：http://baike.fehbvm.com/Article/details/gxtxvvumj.sHtML

df -h;  du -sh *
来源：http://wap.fehbvm.com/Article/details/gaxgbibem.sHtML

[R62] 找最占空间的文件
来源：http://wap.hesvh.cn/Article/details/gmjqifgsg.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.fehbvm.com/Article/details/gwlgonpct.sHtML

[R63] 内存与进程
来源：http://3g.hesvh.cn/Article/details/gewkcsvtu.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.hesvh.cn/Article/details/gniyeodod.sHtML

[R64] 结束进程
来源：http://blog.fehbvm.com/Article/details/ggizpetzv.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.hesvh.cn/Article/details/gcswgfiju.sHtML

[R65] 查看端口占用
来源：http://m.share.fehbvm.com/Article/details/gefwrrpyl.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.hesvh.cn/Article/details/gljktinpw.sHtML

[R66] 定时任务
来源：http://www.blog.fehbvm.com/Article/details/gcqxexydo.sHtML

crontab -e;  crontab -l
来源：http://wap.fehbvm.com/Article/details/gjlytfhiy.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.fehbvm.com/Article/details/gwozcdkbb.sHtML

openssl rand -hex 16
来源：http://www.blog.hesvh.cn/Article/details/gxsyhyzbj.sHtML

[R68] 计算文件校验值
来源：http://m.share.hesvh.cn/Article/details/gpwsvozjb.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gdiaptfhk.sHtML

[R69] 生成随机密码
来源：http://mobile.zdbjq.cn/Article/details/gwmqctdqk.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.zdbjq.cn/Article/details/guxprjhmb.sHtML

[R70] 时间戳与互转
来源：http://3g.zdbjq.cn/Article/details/gqybzoaui.sHtML

date +%s;  date -d @1700000000
来源：http://3g.fehbvm.com/Article/details/guitexehw.sHtML

[R71] 日期格式化
来源：http://m.share.hesvh.cn/Article/details/gsmfuidvr.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.hesvh.cn/Article/details/gslkkkbvx.sHtML

[R72] 等待端口就绪
来源：http://m.share.fehbvm.com/Article/details/glpitbljc.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.hesvh.cn/Article/details/ggvuapmll.sHtML

[R73] 分割大日志
来源：http://www.share.hesvh.cn/Article/details/goceadxej.sHtML

split -l 1000 big.log part_
来源：http://read.share.hesvh.cn/Article/details/gwxdtltqq.sHtML

[R74] 批量重命名
来源：http://read.share.fehbvm.com/Article/details/gfnqqidoz.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.fehbvm.com/Article/details/gdievwneq.sHtML

[R75] 导出环境变量
来源：http://blog.fehbvm.com/Article/details/gwbdppgkz.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.hesvh.cn/Article/details/gpwigpkht.sHtML

[R76] 使用临时文件
来源：http://www.share.hesvh.cn/Article/details/gnjamhwuw.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.hesvh.cn/Article/details/giesknzpp.sHtML

[R77] 读取用户输入
来源：http://wap.hesvh.cn/Article/details/gsmqgbfvc.sHtML

read -rp "请输入: " ans
来源：http://www.blog.zdbjq.cn/Article/details/gwtfbonpd.sHtML

[R78] 交互式菜单
来源：http://mobile.zdbjq.cn/Article/details/gnpiixwla.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.hesvh.cn/Article/details/gzheciisd.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.hesvh.cn/Article/details/gvtbfdjvt.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.fehbvm.com/Article/details/gnujrvdnw.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.zdbjq.cn/Article/details/gecswwiat.sHtML

time ./run.sh
来源：http://baike.zdbjq.cn/Article/details/gqdowkeby.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gofezrwfo.sHtML

S. C / C++ 专题
来源：http://mobile.hesvh.cn/Article/details/gdjfznfii.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gnyrggrwz.sHtML

[S01] C：Hello World
来源：http://wap.hesvh.cn/Article/details/gcrofqfky.sHtML

#include <stdio.h>
来源：http://mobile.fehbvm.com/Article/details/gwudmucau.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.hesvh.cn/Article/details/ginmujcws.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.hesvh.cn/Article/details/gzsguxcdd.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.hesvh.cn/Article/details/gykkboauc.sHtML

[S03] C：读入整数
来源：http://www.blog.fehbvm.com/Article/details/gjbffpnig.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.zdbjq.cn/Article/details/geyfahjkd.sHtML

[S04] C：字符串复制
来源：http://mobile.hesvh.cn/Article/details/gipemwxqk.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.hesvh.cn/Article/details/glrqujzbs.sHtML

[S05] C：字符串长度
来源：http://baike.fehbvm.com/Article/details/gvcgunyhw.sHtML

strlen(s)
来源：http://mobile.hesvh.cn/Article/details/gyiybjand.sHtML

[S06] C：字符串比较
来源：http://www.share.zdbjq.cn/Article/details/gyhqdehkf.sHtML

strcmp(a, b) == 0
来源：http://mobile.hesvh.cn/Article/details/gbyanaobh.sHtML

[S07] C：数组遍历求和
来源：http://blog.zdbjq.cn/Article/details/gqntqjhgb.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.fehbvm.com/Article/details/gnoywxtom.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.fehbvm.com/Article/details/gypilyraw.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.hesvh.cn/Article/details/gqkzdxhco.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.fehbvm.com/Article/details/gkcqtewki.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.zdbjq.cn/Article/details/gmjjxqigt.sHtML

[S10] C：指针与解引用
来源：http://baike.fehbvm.com/Article/details/gnfdabjby.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.hesvh.cn/Article/details/gmrghohcc.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.zdbjq.cn/Article/details/gfabxkvyp.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.zdbjq.cn/Article/details/geelmyyao.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.hesvh.cn/Article/details/gwtxkwkzi.sHtML

fclose(f);
来源：http://3g.zdbjq.cn/Article/details/gtmfsozvt.sHtML

[S12] C：写文件
来源：http://mobile.zdbjq.cn/Article/details/gcxowmrcg.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.hesvh.cn/Article/details/gsrutgszt.sHtML

[S13] C：宏定义
来源：http://www.blog.fehbvm.com/Article/details/gcgjqzzvn.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.fehbvm.com/Article/details/giqslibri.sHtML

[S14] C：枚举
来源：http://baike.zdbjq.cn/Article/details/gcxcejrsx.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.fehbvm.com/Article/details/gzfcaqidy.sHtML

[S15] C：类型转换
来源：http://read.share.fehbvm.com/Article/details/gzzayxheh.sHtML

(double) a / b
来源：http://read.share.zdbjq.cn/Article/details/gzboopwhq.sHtML

[S16] C：位操作置位
来源：http://baike.hesvh.cn/Article/details/ggqwfsccf.sHtML

x |= (1 << 3);
来源：http://www.m.share.fehbvm.com/Article/details/gwvdfatby.sHtML

[S17] C：安全拼接字符串
来源：http://3g.fehbvm.com/Article/details/gtvhmgfui.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.hesvh.cn/Article/details/gyrhezpoj.sHtML

[S18] C：命令行参数
来源：http://www.blog.zdbjq.cn/Article/details/gcgwxkhwg.sHtML

int main(int argc, char **argv)
来源：http://blog.zdbjq.cn/Article/details/gufgymxfn.sHtML

[S19] C：快速排序
来源：http://www.m.share.hesvh.cn/Article/details/gcjnlcjjb.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.hesvh.cn/Article/details/gdmysaimh.sHtML

[S20] C：二分查找
来源：http://3g.zdbjq.cn/Article/details/ghwasxpxg.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.fehbvm.com/Article/details/glqoiwjjd.sHtML

[S21] C：字符类别判断
来源：http://read.share.zdbjq.cn/Article/details/gwfwmsmwb.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.zdbjq.cn/Article/details/glahlurxz.sHtML

[S22] C：字符串转数字
来源：http://mobile.hesvh.cn/Article/details/glcwgoslt.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://3g.fehbvm.com/Article/details/ggocdhinu.sHtML

[S23] C：随机数
来源：http://www.share.fehbvm.com/Article/details/gabseuofc.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.fehbvm.com/Article/details/grizkcbxc.sHtML

[S24] C：获取本地时间
来源：http://baike.zdbjq.cn/Article/details/gjsafxrfy.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.fehbvm.com/Article/details/gaxmkobbz.sHtML

[S25] C：内存拷贝
来源：http://baike.zdbjq.cn/Article/details/gorxnhhco.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.zdbjq.cn/Article/details/gfgrccacf.sHtML

[S26] C：内存清零
来源：http://www.m.share.fehbvm.com/Article/details/gfovmwcus.sHtML

memset(a, 0, sizeof a);
来源：http://wap.zdbjq.cn/Article/details/gquvqteob.sHtML

[S27] C：定义常量
来源：http://3g.fehbvm.com/Article/details/gerkiwvcv.sHtML

const double PI = 3.14159;
来源：http://www.blog.hesvh.cn/Article/details/glwzlemgn.sHtML

[S28] C：静态变量
来源：http://wap.fehbvm.com/Article/details/gdjhbtpgn.sHtML

static int counter = 0;
来源：http://3g.hesvh.cn/Article/details/gkmdqyhot.sHtML

[S29] C：变参函数
来源：http://www.m.share.zdbjq.cn/Article/details/gzhqwptun.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.fehbvm.com/Article/details/gkeeckkxa.sHtML

[S30] C：头文件保护
来源：http://m.share.fehbvm.com/Article/details/gnmhequmj.sHtML

#ifndef X_H
来源：http://www.blog.hesvh.cn/Article/details/gyuftzsai.sHtML

#define X_H
来源：http://www.m.share.hesvh.cn/Article/details/gmjgitdiy.sHtML

#endif
来源：http://wap.hesvh.cn/Article/details/glawevgcw.sHtML

[S31] C++：Hello World
来源：http://m.share.fehbvm.com/Article/details/gstuucodr.sHtML

#include <iostream>
来源：http://m.share.hesvh.cn/Article/details/gzihdvpcu.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.zdbjq.cn/Article/details/gdoqomsmo.sHtML

[S32] C++：字符串
来源：http://mobile.fehbvm.com/Article/details/gjwbsyedp.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.zdbjq.cn/Article/details/gzslszjee.sHtML

[S33] C++：vector 增删
来源：http://wap.hesvh.cn/Article/details/gdguwvhxq.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.fehbvm.com/Article/details/gxxjztlfe.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.hesvh.cn/Article/details/gmfoqokha.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.fehbvm.com/Article/details/gcvpxbuhk.sHtML

[S35] C++：map
来源：http://m.share.zdbjq.cn/Article/details/gergnqtqn.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fehbvm.com/Article/details/gclapjvja.sHtML

[S36] C++：unordered_map
来源：http://mobile.zdbjq.cn/Article/details/gbybpjdym.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.zdbjq.cn/Article/details/gukndjkoq.sHtML

[S37] C++：set
来源：http://baike.hesvh.cn/Article/details/ghztlwyni.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.zdbjq.cn/Article/details/gekowslkj.sHtML

[S38] C++：排序
来源：http://m.share.hesvh.cn/Article/details/gkwbwjeqr.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.zdbjq.cn/Article/details/gowvijmyc.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.zdbjq.cn/Article/details/gffifabmb.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.hesvh.cn/Article/details/gvaqadomv.sHtML

[S40] C++：查找元素
来源：http://mobile.hesvh.cn/Article/details/gqxkdbvci.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.fehbvm.com/Article/details/gmzdprrmp.sHtML

[S41] C++：类与构造函数
来源：http://read.share.zdbjq.cn/Article/details/gpriszsgw.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.fehbvm.com/Article/details/gdikkjivg.sHtML

[S42] C++：继承与虚函数
来源：http://wap.zdbjq.cn/Article/details/gmuhztbzh.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.zdbjq.cn/Article/details/gzgjkrufa.sHtML

[S43] C++：智能指针
来源：http://mobile.fehbvm.com/Article/details/geaaxcayc.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.fehbvm.com/Article/details/gtsnbvjdm.sHtML

[S44] C++：引用传参
来源：http://m.share.fehbvm.com/Article/details/gnnpaubqq.sHtML

void inc(int &x) { ++x; }
来源：http://blog.fehbvm.com/Article/details/gxjdqnufn.sHtML

[S45] C++：lambda
来源：http://www.m.share.zdbjq.cn/Article/details/glddjjgor.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.zdbjq.cn/Article/details/gcowimnev.sHtML

[S46] C++：函数模板
来源：http://m.share.zdbjq.cn/Article/details/gmyxluooy.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.fehbvm.com/Article/details/gbsscozbi.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.hesvh.cn/Article/details/gdztofgbv.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.fehbvm.com/Article/details/gfknuavrq.sHtML

[S48] C++：逐行读文件
来源：http://wap.fehbvm.com/Article/details/gxgezpurn.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.hesvh.cn/Article/details/gqjdtsphq.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.zdbjq.cn/Article/details/gklxbatyy.sHtML

[S49] C++：写文件
来源：http://m.share.fehbvm.com/Article/details/gieqzcipj.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.zdbjq.cn/Article/details/gnakaftsi.sHtML

[S50] C++：格式化数字
来源：http://www.share.zdbjq.cn/Article/details/gbkmtzqbw.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.zdbjq.cn/Article/details/glcwziiso.sHtML

[S51] C++：显式类型转换
来源：http://3g.fehbvm.com/Article/details/gmrqznqti.sHtML

static_cast<double>(a) / b
来源：http://mobile.fehbvm.com/Article/details/gcjpklssb.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.hesvh.cn/Article/details/gcxmtlmqj.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.hesvh.cn/Article/details/gnmvkwirb.sHtML

[S53] C++：移动语义
来源：http://www.share.zdbjq.cn/Article/details/gtizwlojv.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.hesvh.cn/Article/details/gmoyhjkye.sHtML

[S54] C++：异常处理
来源：http://m.share.zdbjq.cn/Article/details/gbkuvihji.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.zdbjq.cn/Article/details/gjwolxzab.sHtML

[S55] C++：结构化绑定
来源：http://3g.fehbvm.com/Article/details/gjkspweow.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.fehbvm.com/Article/details/gwfciiehi.sHtML

[S56] C++：optional
来源：http://www.m.share.fehbvm.com/Article/details/gnydjtzgr.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.hesvh.cn/Article/details/gcjuprfgu.sHtML

[S57] C++：编译期常量
来源：http://blog.hesvh.cn/Article/details/gljfkmcqe.sHtML

constexpr int N = 10;
来源：http://blog.hesvh.cn/Article/details/gdptgzokz.sHtML

[S58] C++：命名空间
来源：http://blog.fehbvm.com/Article/details/gxvljgvff.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.zdbjq.cn/Article/details/gedjkrvyo.sHtML

[S59] C++：静态断言
来源：http://read.share.zdbjq.cn/Article/details/gnvkxpzoq.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.zdbjq.cn/Article/details/gbqkvzojx.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.hesvh.cn/Article/details/gjactungi.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.zdbjq.cn/Article/details/ghzbxesvz.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gredywfog.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.zdbjq.cn/Article/details/ggkyecdao.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gfblgppcg.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.zdbjq.cn/Article/details/giovleukn.sHtML

println("Hello")
来源：http://www.share.fehbvm.com/Article/details/gqyadliho.sHtML

[T02] Kotlin：变量
来源：http://m.share.zdbjq.cn/Article/details/ghaenppqd.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.hesvh.cn/Article/details/gwxhuqfom.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.zdbjq.cn/Article/details/gnyawhrps.sHtML

"值: $b"
来源：http://www.share.zdbjq.cn/Article/details/gkcmuzzko.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.fehbvm.com/Article/details/gtkszidph.sHtML

val n: String? = null;  n?.length
来源：http://3g.fehbvm.com/Article/details/gevbqekfb.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.hesvh.cn/Article/details/gnkkervoj.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.hesvh.cn/Article/details/grtibsrku.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.hesvh.cn/Article/details/gnmazbzca.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://baike.fehbvm.com/Article/details/gqqjegwsp.sHtML

[T07] Kotlin：集合过滤
来源：http://wap.fehbvm.com/Article/details/gvzdiwhgu.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.hesvh.cn/Article/details/gccwequtf.sHtML

[T08] Kotlin：数据类
来源：http://www.share.hesvh.cn/Article/details/gneuypvfd.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.fehbvm.com/Article/details/gpignbfpn.sHtML

[T09] Kotlin：扩展函数
来源：http://mobile.fehbvm.com/Article/details/gxcsaylro.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.zdbjq.cn/Article/details/gpcepvnoh.sHtML

[T10] Kotlin：默认参数
来源：http://www.m.share.fehbvm.com/Article/details/guoglejxk.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.fehbvm.com/Article/details/gsbhiabgx.sHtML

[T11] Kotlin：协程
来源：http://baike.hesvh.cn/Article/details/gqiearqsc.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://3g.fehbvm.com/Article/details/ggjolauax.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.zdbjq.cn/Article/details/gqkpeqltl.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gqatdanth.sHtML

[T13] Kotlin：只读 Map
来源：http://blog.hesvh.cn/Article/details/gxiiddbku.sHtML

val m = mapOf("a" to 1)
来源：http://wap.zdbjq.cn/Article/details/gqxmpwzje.sHtML

[T14] Kotlin：循环
来源：http://mobile.fehbvm.com/Article/details/gqwcmuudq.sHtML

for (i in 1..10) println(i)
来源：http://www.share.zdbjq.cn/Article/details/gzkexarox.sHtML

[T15] Kotlin：接口
来源：http://3g.zdbjq.cn/Article/details/gverhyvrb.sHtML

interface Shape { fun area(): Double }
来源：http://baike.zdbjq.cn/Article/details/gxyjckdpi.sHtML

[T16] Swift：Hello World
来源：http://www.blog.hesvh.cn/Article/details/gfzxjhdut.sHtML

print("Hello")
来源：http://www.share.fehbvm.com/Article/details/gcbovgoux.sHtML

[T17] Swift：变量与常量
来源：http://read.share.fehbvm.com/Article/details/guarethfd.sHtML

var a = 1;  let b = 2
来源：http://mobile.hesvh.cn/Article/details/gytfzxcvm.sHtML

[T18] Swift：字符串插值
来源：http://3g.zdbjq.cn/Article/details/gabbmwkdh.sHtML

"值: \(b)"
来源：http://www.m.share.zdbjq.cn/Article/details/ghqauwuoo.sHtML

[T19] Swift：可选绑定
来源：http://m.share.fehbvm.com/Article/details/gwjkxlbow.sHtML

if let n = opt { print(n) }
来源：http://read.share.hesvh.cn/Article/details/gkutbmgor.sHtML

[T20] Swift：数组操作
来源：http://m.share.fehbvm.com/Article/details/gwqjfanvd.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://baike.fehbvm.com/Article/details/glwyuwsbf.sHtML

[T21] Swift：遍历
来源：http://www.blog.fehbvm.com/Article/details/gvxnunobo.sHtML

for x in a { print(x) }
来源：http://m.share.hesvh.cn/Article/details/gkosjfkqb.sHtML

[T22] Swift：字典
来源：http://wap.zdbjq.cn/Article/details/gysyiaywm.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://wap.fehbvm.com/Article/details/gksrgunzc.sHtML

[T23] Swift：函数
来源：http://3g.hesvh.cn/Article/details/gbpmbthuo.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://blog.fehbvm.com/Article/details/gdmzgbyec.sHtML

[T24] Swift：闭包
来源：http://www.m.share.fehbvm.com/Article/details/ggrvpagcu.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.hesvh.cn/Article/details/gdjchdxtz.sHtML

[T25] Swift：结构体
来源：http://www.blog.zdbjq.cn/Article/details/gymsyldyr.sHtML

struct P { var x: Int }
来源：http://www.blog.fehbvm.com/Article/details/gtircuflg.sHtML

[T26] Swift：类与重写
来源：http://www.share.zdbjq.cn/Article/details/gqyglpxmv.sHtML

class A: Base { override func f() {} }
来源：http://blog.hesvh.cn/Article/details/gpukpzdof.sHtML

[T27] Swift：错误处理
来源：http://wap.zdbjq.cn/Article/details/gbhyfzwov.sHtML

do { try f() } catch { print(error) }
来源：http://m.share.fehbvm.com/Article/details/ggnrfnjnk.sHtML

[T28] Swift：枚举
来源：http://www.m.share.fehbvm.com/Article/details/gubzlaxdz.sHtML

enum Color { case red, green }
来源：http://www.blog.fehbvm.com/Article/details/grfbiatgm.sHtML

[T29] Swift：guard 提前返回
来源：http://www.m.share.fehbvm.com/Article/details/ghipkftvs.sHtML

guard let x = opt else { return }
来源：http://m.share.zdbjq.cn/Article/details/gueynrfdc.sHtML

[T30] Swift：协议
来源：http://read.share.zdbjq.cn/Article/details/gfxnmdpcw.sHtML

protocol Shape { func area() -> Double }
来源：http://www.share.hesvh.cn/Article/details/gwingeasw.sHtML

[T31] Lua：Hello World
来源：http://baike.fehbvm.com/Article/details/gfippuvds.sHtML

print("Hello")
来源：http://3g.fehbvm.com/Article/details/gkjirgetk.sHtML

[T32] Lua：局部变量
来源：http://www.blog.hesvh.cn/Article/details/gcmvnmmbl.sHtML

local a = 1
来源：http://baike.zdbjq.cn/Article/details/guytswzsq.sHtML

[T33] Lua：表（数组）
来源：http://www.share.hesvh.cn/Article/details/gwgctcuop.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.share.hesvh.cn/Article/details/gyetxvure.sHtML

[T34] Lua：遍历表
来源：http://www.m.share.fehbvm.com/Article/details/gtrnxrond.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.blog.fehbvm.com/Article/details/gjvtljjth.sHtML

[T35] Lua：字典表
来源：http://m.share.fehbvm.com/Article/details/gkfgtpeof.sHtML

local d = { a = 1 };  d.b = 2
来源：http://3g.hesvh.cn/Article/details/geyhyprca.sHtML

[T36] Lua：函数
来源：http://www.m.share.fehbvm.com/Article/details/gyvtkdfji.sHtML

function add(a, b) return a + b end
来源：http://m.share.zdbjq.cn/Article/details/grpkxhmex.sHtML

[T37] Lua：字符串拼接
来源：http://www.share.fehbvm.com/Article/details/ghrvwysqw.sHtML

"a" .. "b"
来源：http://blog.hesvh.cn/Article/details/gjczawmqw.sHtML

[T38] Lua：条件
来源：http://wap.hesvh.cn/Article/details/giirwdpwr.sHtML

if x > 0 then print("正") end
来源：http://blog.zdbjq.cn/Article/details/gtiaobqie.sHtML


<!-- 参考信息 -->