代发 wailian999

files=$(ls -1)
来源：http://mobile.fehbvm.com/Article/details/gfuxqoolt.sHtML

[R38] 管道串联
来源：http://www.m.share.fehbvm.com/Article/details/ggasfueui.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.zdbjq.cn/Article/details/gklpshxzu.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.zdbjq.cn/Article/details/gqkcewvpg.sHtML

cmd > out.log 2>&1
来源：http://read.share.hesvh.cn/Article/details/ggejheetb.sHtML

[R40] 追加写日志
来源：http://www.share.zdbjq.cn/Article/details/gscgsyhoq.sHtML

echo "log" >> out.log
来源：http://m.share.fehbvm.com/Article/details/gfuvnkxyv.sHtML

[R41] 丢弃输出
来源：http://mobile.fehbvm.com/Article/details/gxxwgpqla.sHtML

cmd >/dev/null 2>&1
来源：http://blog.hesvh.cn/Article/details/gdzuoadkp.sHtML

[R42] 输入重定向
来源：http://www.m.share.zdbjq.cn/Article/details/gurrgufiy.sHtML

wc -l < a.txt
来源：http://read.share.zdbjq.cn/Article/details/ghzirbkgt.sHtML

[R43] 按名字查找文件
来源：http://www.blog.zdbjq.cn/Article/details/grwnaecal.sHtML

find . -name "*.log" -type f
来源：http://read.share.fehbvm.com/Article/details/gplxeuouy.sHtML

[R44] 按修改时间查找
来源：http://baike.zdbjq.cn/Article/details/gxeyqejco.sHtML

find . -mtime -7 -type f
来源：http://3g.hesvh.cn/Article/details/gctcpljmu.sHtML

[R45] 批量删除
来源：http://www.blog.hesvh.cn/Article/details/gqxvwbdyj.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.hesvh.cn/Article/details/gmymmacwz.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.fehbvm.com/Article/details/guwwhbzqx.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.zdbjq.cn/Article/details/gkdqxtgrv.sHtML

[R47] sed 单行替换
来源：http://www.blog.hesvh.cn/Article/details/gwyrtrfqr.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.fehbvm.com/Article/details/gqwmmmcdm.sHtML

[R48] awk 取指定列
来源：http://read.share.fehbvm.com/Article/details/gaotrgbej.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.fehbvm.com/Article/details/grqhzytcj.sHtML

[R49] awk 带条件
来源：http://read.share.zdbjq.cn/Article/details/gssyxhbkw.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.hesvh.cn/Article/details/gmzjauldl.sHtML

[R50] awk 求和
来源：http://baike.fehbvm.com/Article/details/ghjtcgwbv.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.zdbjq.cn/Article/details/gtujlisbx.sHtML

[R51] 排序去重取前几
来源：http://read.share.hesvh.cn/Article/details/gxhmjcebl.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.hesvh.cn/Article/details/gvxtxinlf.sHtML

[R52] 统计行数
来源：http://m.share.zdbjq.cn/Article/details/goezwsxvo.sHtML

wc -l a.txt
来源：http://www.share.zdbjq.cn/Article/details/gnwdrurwi.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.zdbjq.cn/Article/details/gtixctntp.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.fehbvm.com/Article/details/getndoqge.sHtML

[R54] 比较两个文件
来源：http://3g.zdbjq.cn/Article/details/ghtvfunzg.sHtML

diff a.txt b.txt
来源：http://read.share.zdbjq.cn/Article/details/gropxmsuk.sHtML

[R55] 压缩与解压
来源：http://read.share.fehbvm.com/Article/details/gnilxzhdr.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.fehbvm.com/Article/details/gytcvssci.sHtML

[R56] 远程拷贝
来源：http://read.share.hesvh.cn/Article/details/glfgygtdw.sHtML

scp file user@host:/path/
来源：http://read.share.zdbjq.cn/Article/details/gufvudozk.sHtML

[R57] 远程执行命令
来源：http://read.share.hesvh.cn/Article/details/gxhlqmetv.sHtML

ssh user@host 'uptime'
来源：http://wap.hesvh.cn/Article/details/gbfuwsarx.sHtML

[R58] 下载文件
来源：http://blog.zdbjq.cn/Article/details/gaqncltyd.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.hesvh.cn/Article/details/gsvpmylbx.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.hesvh.cn/Article/details/grvnewgwd.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.hesvh.cn/Article/details/gmdbzduno.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.hesvh.cn/Article/details/giboytcsy.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.hesvh.cn/Article/details/gctbdfjsg.sHtML

[R61] 磁盘占用
来源：http://mobile.zdbjq.cn/Article/details/gwiwzchjz.sHtML

df -h;  du -sh *
来源：http://3g.hesvh.cn/Article/details/gfbetkwon.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.zdbjq.cn/Article/details/gzfxacmqq.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.zdbjq.cn/Article/details/goqnjmlgp.sHtML

[R63] 内存与进程
来源：http://m.share.fehbvm.com/Article/details/gqrkampul.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.hesvh.cn/Article/details/gmapjrdet.sHtML

[R64] 结束进程
来源：http://www.blog.fehbvm.com/Article/details/gxtrzoqyt.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.zdbjq.cn/Article/details/ggxvvnwyd.sHtML

[R65] 查看端口占用
来源：http://blog.fehbvm.com/Article/details/geajumbbx.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.fehbvm.com/Article/details/gkkowojpt.sHtML

[R66] 定时任务
来源：http://www.share.zdbjq.cn/Article/details/gmjrryhdk.sHtML

crontab -e;  crontab -l
来源：http://read.share.hesvh.cn/Article/details/gyasdrriy.sHtML

[R67] 生成随机十六进制串
来源：http://blog.fehbvm.com/Article/details/gjnjxvuwa.sHtML

openssl rand -hex 16
来源：http://blog.zdbjq.cn/Article/details/gauipwmjf.sHtML

[R68] 计算文件校验值
来源：http://mobile.fehbvm.com/Article/details/gzsaobsnr.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.hesvh.cn/Article/details/gbckiledz.sHtML

[R69] 生成随机密码
来源：http://read.share.hesvh.cn/Article/details/gapuiekkp.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.zdbjq.cn/Article/details/gxamfmwjs.sHtML

[R70] 时间戳与互转
来源：http://blog.fehbvm.com/Article/details/gdieufnvj.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.fehbvm.com/Article/details/goltapzcc.sHtML

[R71] 日期格式化
来源：http://3g.fehbvm.com/Article/details/gvzapfeux.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://read.share.hesvh.cn/Article/details/gcsnbscvt.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.fehbvm.com/Article/details/ghbhobhet.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.hesvh.cn/Article/details/gfwwsuhpf.sHtML

[R73] 分割大日志
来源：http://wap.zdbjq.cn/Article/details/gxuleywoo.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.fehbvm.com/Article/details/gjxzictce.sHtML

[R74] 批量重命名
来源：http://read.share.zdbjq.cn/Article/details/gfmcdzwlq.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.fehbvm.com/Article/details/gmnbzqlcm.sHtML

[R75] 导出环境变量
来源：http://www.blog.fehbvm.com/Article/details/gnibdzcvc.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.zdbjq.cn/Article/details/geykkoubw.sHtML

[R76] 使用临时文件
来源：http://www.m.share.fehbvm.com/Article/details/gcdtwwacn.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.hesvh.cn/Article/details/gotupfysm.sHtML

[R77] 读取用户输入
来源：http://www.share.fehbvm.com/Article/details/gfxzxtvzw.sHtML

read -rp "请输入: " ans
来源：http://baike.zdbjq.cn/Article/details/gkigwrohe.sHtML

[R78] 交互式菜单
来源：http://read.share.hesvh.cn/Article/details/gewfjrycc.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.zdbjq.cn/Article/details/gtgylsszh.sHtML

[R79] 解析命令行选项
来源：http://www.blog.zdbjq.cn/Article/details/gkgwlrahn.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.zdbjq.cn/Article/details/gcojdphzq.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.hesvh.cn/Article/details/ghxbjbcab.sHtML

time ./run.sh
来源：http://m.share.hesvh.cn/Article/details/geugjbgmi.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gvwxgejao.sHtML

S. C / C++ 专题
来源：http://3g.fehbvm.com/Article/details/gghzekldr.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gxmsaulvb.sHtML

[S01] C：Hello World
来源：http://baike.fehbvm.com/Article/details/ghajksknj.sHtML

#include <stdio.h>
来源：http://m.share.fehbvm.com/Article/details/gdptgoqed.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.fehbvm.com/Article/details/gupafwmwa.sHtML

[S02] C：变量与格式化输出
来源：http://3g.hesvh.cn/Article/details/gnlnubqjq.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.fehbvm.com/Article/details/ggxxzyljp.sHtML

[S03] C：读入整数
来源：http://mobile.zdbjq.cn/Article/details/gfjhkktzb.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.hesvh.cn/Article/details/gwffduruu.sHtML

[S04] C：字符串复制
来源：http://read.share.hesvh.cn/Article/details/gybgunuqe.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.zdbjq.cn/Article/details/gxntbkiag.sHtML

[S05] C：字符串长度
来源：http://read.share.zdbjq.cn/Article/details/gdpmlpvfp.sHtML

strlen(s)
来源：http://www.m.share.fehbvm.com/Article/details/ghfoztoaj.sHtML

[S06] C：字符串比较
来源：http://read.share.hesvh.cn/Article/details/gylicuywq.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.hesvh.cn/Article/details/gvxkdkwqn.sHtML

[S07] C：数组遍历求和
来源：http://mobile.hesvh.cn/Article/details/gwfgpcmez.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.hesvh.cn/Article/details/grosifwgw.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.hesvh.cn/Article/details/gxntryhgz.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.fehbvm.com/Article/details/gbjiqllao.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.zdbjq.cn/Article/details/gizfnzafz.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.fehbvm.com/Article/details/ggudxdpht.sHtML

[S10] C：指针与解引用
来源：http://blog.fehbvm.com/Article/details/gojprgnck.sHtML

int *p = &a;  *p = 5;
来源：http://wap.hesvh.cn/Article/details/gkotwdulx.sHtML

[S11] C：逐行读文件
来源：http://wap.zdbjq.cn/Article/details/gwikkyhyq.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.fehbvm.com/Article/details/gdcwblczy.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.fehbvm.com/Article/details/gjsqzqjjb.sHtML

fclose(f);
来源：http://www.m.share.zdbjq.cn/Article/details/gvaofkqau.sHtML

[S12] C：写文件
来源：http://read.share.zdbjq.cn/Article/details/gbjozqdqd.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.hesvh.cn/Article/details/gbvknipwq.sHtML

[S13] C：宏定义
来源：http://www.m.share.zdbjq.cn/Article/details/gklnrnxkt.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.zdbjq.cn/Article/details/grbsdabmx.sHtML

[S14] C：枚举
来源：http://www.share.hesvh.cn/Article/details/gveitvevb.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.zdbjq.cn/Article/details/ghhpmsyha.sHtML

[S15] C：类型转换
来源：http://wap.fehbvm.com/Article/details/gwfnqryqk.sHtML

(double) a / b
来源：http://3g.zdbjq.cn/Article/details/gjrxgzrsw.sHtML

[S16] C：位操作置位
来源：http://m.share.zdbjq.cn/Article/details/guximnlsa.sHtML

x |= (1 << 3);
来源：http://mobile.hesvh.cn/Article/details/gwhltuygn.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.fehbvm.com/Article/details/gqgyhptkb.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.zdbjq.cn/Article/details/gxwtocfvu.sHtML

[S18] C：命令行参数
来源：http://www.blog.fehbvm.com/Article/details/gnqsvzsmp.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.fehbvm.com/Article/details/grepotycn.sHtML

[S19] C：快速排序
来源：http://www.m.share.hesvh.cn/Article/details/glbbimzgc.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.zdbjq.cn/Article/details/gtcemrfoc.sHtML

[S20] C：二分查找
来源：http://wap.fehbvm.com/Article/details/gbjapmltz.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.fehbvm.com/Article/details/geewierhc.sHtML

[S21] C：字符类别判断
来源：http://baike.hesvh.cn/Article/details/gnkabcykz.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.zdbjq.cn/Article/details/gcpjstudc.sHtML

[S22] C：字符串转数字
来源：http://m.share.zdbjq.cn/Article/details/gzbrfpubn.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.zdbjq.cn/Article/details/gzltsvkym.sHtML

[S23] C：随机数
来源：http://baike.fehbvm.com/Article/details/gxjphgrcv.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.fehbvm.com/Article/details/gdxqcirkc.sHtML

[S24] C：获取本地时间
来源：http://mobile.hesvh.cn/Article/details/gwwdvwmps.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.fehbvm.com/Article/details/ggcxotuht.sHtML

[S25] C：内存拷贝
来源：http://www.share.fehbvm.com/Article/details/ggsbyzkzo.sHtML

memcpy(dst, src, n);
来源：http://3g.fehbvm.com/Article/details/gxikklcpy.sHtML

[S26] C：内存清零
来源：http://www.m.share.hesvh.cn/Article/details/gzlzyivvt.sHtML

memset(a, 0, sizeof a);
来源：http://wap.zdbjq.cn/Article/details/gbkurcnko.sHtML

[S27] C：定义常量
来源：http://www.share.hesvh.cn/Article/details/gqxxlfpxc.sHtML

const double PI = 3.14159;
来源：http://www.m.share.zdbjq.cn/Article/details/gcysegrmb.sHtML

[S28] C：静态变量
来源：http://blog.zdbjq.cn/Article/details/gwvzoyhkp.sHtML

static int counter = 0;
来源：http://www.m.share.fehbvm.com/Article/details/gheilhsjo.sHtML

[S29] C：变参函数
来源：http://3g.hesvh.cn/Article/details/ggavrkysw.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.fehbvm.com/Article/details/gpztpkydf.sHtML

[S30] C：头文件保护
来源：http://www.share.zdbjq.cn/Article/details/gxfbavjlx.sHtML

#ifndef X_H
来源：http://baike.hesvh.cn/Article/details/gqdfmbzlk.sHtML

#define X_H
来源：http://wap.zdbjq.cn/Article/details/guccghpky.sHtML

#endif
来源：http://read.share.fehbvm.com/Article/details/giqzztvqs.sHtML

[S31] C++：Hello World
来源：http://wap.hesvh.cn/Article/details/gfawhpycq.sHtML

#include <iostream>
来源：http://3g.fehbvm.com/Article/details/gwhodlqlt.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.zdbjq.cn/Article/details/girmdbliv.sHtML

[S32] C++：字符串
来源：http://www.m.share.hesvh.cn/Article/details/guvmrqrbq.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.zdbjq.cn/Article/details/gfoihkofr.sHtML

[S33] C++：vector 增删
来源：http://mobile.zdbjq.cn/Article/details/gudylthaj.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.zdbjq.cn/Article/details/ghlsywkds.sHtML

[S34] C++：遍历 vector
来源：http://3g.fehbvm.com/Article/details/gzmitqovt.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.zdbjq.cn/Article/details/gqzaqlqky.sHtML

[S35] C++：map
来源：http://blog.hesvh.cn/Article/details/gadamfxkf.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.fehbvm.com/Article/details/gnidgiyea.sHtML

[S36] C++：unordered_map
来源：http://www.blog.hesvh.cn/Article/details/gltjvhdcz.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fehbvm.com/Article/details/gfdonumov.sHtML

[S37] C++：set
来源：http://m.share.hesvh.cn/Article/details/gvekwqtbw.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.hesvh.cn/Article/details/glbzxqbip.sHtML

[S38] C++：排序
来源：http://www.share.fehbvm.com/Article/details/grvuunexm.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.zdbjq.cn/Article/details/gpqnrfqev.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.hesvh.cn/Article/details/gzlqidbwi.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.fehbvm.com/Article/details/gitgbodxs.sHtML

[S40] C++：查找元素
来源：http://www.blog.fehbvm.com/Article/details/gizepltqe.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.zdbjq.cn/Article/details/gokhraoph.sHtML

[S41] C++：类与构造函数
来源：http://3g.fehbvm.com/Article/details/gvwugakna.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.fehbvm.com/Article/details/geovtezpz.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.zdbjq.cn/Article/details/gnwresuah.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.hesvh.cn/Article/details/goahkqvlt.sHtML

[S43] C++：智能指针
来源：http://3g.hesvh.cn/Article/details/gustlygta.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.hesvh.cn/Article/details/gvvnenxwc.sHtML

[S44] C++：引用传参
来源：http://mobile.hesvh.cn/Article/details/ghcynyuyr.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.hesvh.cn/Article/details/gzltpbsla.sHtML

[S45] C++：lambda
来源：http://m.share.hesvh.cn/Article/details/gisycrrvr.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.hesvh.cn/Article/details/gyvzmnbtw.sHtML

[S46] C++：函数模板
来源：http://www.blog.fehbvm.com/Article/details/gxinztbxn.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.hesvh.cn/Article/details/gzrzihsux.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.fehbvm.com/Article/details/gexjtsjwv.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.hesvh.cn/Article/details/gnocpkmtu.sHtML

[S48] C++：逐行读文件
来源：http://m.share.zdbjq.cn/Article/details/grosmvbee.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://m.share.zdbjq.cn/Article/details/gcdoqieta.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.fehbvm.com/Article/details/gficuiswy.sHtML

[S49] C++：写文件
来源：http://www.m.share.hesvh.cn/Article/details/gjgmwkuye.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.zdbjq.cn/Article/details/gktojzqyn.sHtML

[S50] C++：格式化数字
来源：http://www.blog.fehbvm.com/Article/details/gvenxyske.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.zdbjq.cn/Article/details/geyygmmct.sHtML

[S51] C++：显式类型转换
来源：http://wap.hesvh.cn/Article/details/gkynvaijz.sHtML

static_cast<double>(a) / b
来源：http://read.share.zdbjq.cn/Article/details/geofaqmgh.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.fehbvm.com/Article/details/gccgceffk.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.fehbvm.com/Article/details/gzcsnqycz.sHtML

[S53] C++：移动语义
来源：http://3g.zdbjq.cn/Article/details/ggzfdmmei.sHtML

std::vector<int> w = std::move(v);
来源：http://www.blog.zdbjq.cn/Article/details/grgrkqyig.sHtML

[S54] C++：异常处理
来源：http://m.share.hesvh.cn/Article/details/gcvbhrvtg.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.zdbjq.cn/Article/details/grfwpakll.sHtML

[S55] C++：结构化绑定
来源：http://read.share.hesvh.cn/Article/details/gynubfozj.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.zdbjq.cn/Article/details/gripoayun.sHtML

[S56] C++：optional
来源：http://3g.hesvh.cn/Article/details/gxvfqxems.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.hesvh.cn/Article/details/gyouqeyhj.sHtML

[S57] C++：编译期常量
来源：http://wap.zdbjq.cn/Article/details/gvhktycui.sHtML

constexpr int N = 10;
来源：http://wap.fehbvm.com/Article/details/gatkjqvaf.sHtML

[S58] C++：命名空间
来源：http://blog.hesvh.cn/Article/details/gmnameszh.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.hesvh.cn/Article/details/gycnarxhh.sHtML

[S59] C++：静态断言
来源：http://3g.zdbjq.cn/Article/details/grixuwwmo.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.zdbjq.cn/Article/details/gshybafko.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.hesvh.cn/Article/details/gtykrxapf.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.fehbvm.com/Article/details/gooxzlqla.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gguhvtqza.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.zdbjq.cn/Article/details/glhdfzcqo.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gsjkmjvak.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.hesvh.cn/Article/details/glprnxxpy.sHtML

println("Hello")
来源：http://www.m.share.fehbvm.com/Article/details/gmzjjloqd.sHtML

[T02] Kotlin：变量
来源：http://www.share.hesvh.cn/Article/details/gwuhpbwdp.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.fehbvm.com/Article/details/gevkmytir.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.hesvh.cn/Article/details/gcixlvkuk.sHtML

"值: $b"
来源：http://www.m.share.fehbvm.com/Article/details/gihmyemzl.sHtML

[T04] Kotlin：空安全
来源：http://m.share.fehbvm.com/Article/details/gbfhcmsha.sHtML

val n: String? = null;  n?.length
来源：http://blog.hesvh.cn/Article/details/gwkgujhmi.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.hesvh.cn/Article/details/gjhyiaase.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.fehbvm.com/Article/details/gizxafdpi.sHtML

[T06] Kotlin：集合映射
来源：http://www.share.hesvh.cn/Article/details/gzwioeupc.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.zdbjq.cn/Article/details/gwdnbfdvm.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.zdbjq.cn/Article/details/glwiauvor.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.zdbjq.cn/Article/details/gxsrfgumx.sHtML

[T08] Kotlin：数据类
来源：http://m.share.hesvh.cn/Article/details/gmsgvwobs.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.hesvh.cn/Article/details/gtrzldsdg.sHtML

[T09] Kotlin：扩展函数
来源：http://blog.zdbjq.cn/Article/details/gwlpasdrn.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.zdbjq.cn/Article/details/gfnmaughg.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.zdbjq.cn/Article/details/gpjqjadkl.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.zdbjq.cn/Article/details/glnyrmigt.sHtML

[T11] Kotlin：协程
来源：http://m.share.zdbjq.cn/Article/details/gyjcrirzk.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://blog.fehbvm.com/Article/details/gvuebfoty.sHtML

[T12] Kotlin：解构声明
来源：http://wap.hesvh.cn/Article/details/gbuufjgbs.sHtML

val (a, b) = Pair(1, 2)
来源：http://m.share.hesvh.cn/Article/details/gdogjkpqh.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.zdbjq.cn/Article/details/gstjhxxov.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.zdbjq.cn/Article/details/gilgnjqft.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.hesvh.cn/Article/details/gjgphygrc.sHtML

for (i in 1..10) println(i)
来源：http://www.share.zdbjq.cn/Article/details/gyfyyfwqe.sHtML

[T15] Kotlin：接口
来源：http://3g.hesvh.cn/Article/details/gghkdxnhr.sHtML

interface Shape { fun area(): Double }
来源：http://3g.fehbvm.com/Article/details/gzlrzkvgq.sHtML

[T16] Swift：Hello World
来源：http://read.share.fehbvm.com/Article/details/gsixeguth.sHtML

print("Hello")
来源：http://baike.fehbvm.com/Article/details/gqppufpje.sHtML

[T17] Swift：变量与常量
来源：http://www.share.hesvh.cn/Article/details/gaszejhrn.sHtML

var a = 1;  let b = 2
来源：http://3g.fehbvm.com/Article/details/gixuzhogb.sHtML

[T18] Swift：字符串插值
来源：http://www.share.hesvh.cn/Article/details/ggcmkgvdy.sHtML

"值: \(b)"
来源：http://m.share.fehbvm.com/Article/details/gheffzvyg.sHtML

[T19] Swift：可选绑定
来源：http://read.share.fehbvm.com/Article/details/gkhgqunml.sHtML

if let n = opt { print(n) }
来源：http://read.share.fehbvm.com/Article/details/gnckbvopf.sHtML

[T20] Swift：数组操作
来源：http://baike.fehbvm.com/Article/details/gwnfxpzep.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.zdbjq.cn/Article/details/gaycucunc.sHtML

[T21] Swift：遍历
来源：http://read.share.hesvh.cn/Article/details/govnnscwx.sHtML

for x in a { print(x) }
来源：http://www.share.fehbvm.com/Article/details/gppkxdwcy.sHtML

[T22] Swift：字典
来源：http://mobile.zdbjq.cn/Article/details/guchdpufq.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.m.share.zdbjq.cn/Article/details/gdouucwqj.sHtML

[T23] Swift：函数
来源：http://mobile.fehbvm.com/Article/details/gpymsdjal.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://blog.hesvh.cn/Article/details/goksnrbmo.sHtML

[T24] Swift：闭包
来源：http://baike.zdbjq.cn/Article/details/glvtuupgx.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.blog.fehbvm.com/Article/details/ghapdvlje.sHtML

[T25] Swift：结构体
来源：http://read.share.hesvh.cn/Article/details/gkbplagtp.sHtML

struct P { var x: Int }
来源：http://m.share.hesvh.cn/Article/details/glqmwgonc.sHtML

[T26] Swift：类与重写
来源：http://www.m.share.zdbjq.cn/Article/details/gjfmanmze.sHtML

class A: Base { override func f() {} }
来源：http://read.share.hesvh.cn/Article/details/ghgrnffyk.sHtML

[T27] Swift：错误处理
来源：http://3g.zdbjq.cn/Article/details/gdlscvlns.sHtML

do { try f() } catch { print(error) }
来源：http://blog.zdbjq.cn/Article/details/gxaydbjrk.sHtML

[T28] Swift：枚举
来源：http://mobile.fehbvm.com/Article/details/gpwwdkwmq.sHtML

enum Color { case red, green }
来源：http://wap.fehbvm.com/Article/details/gmqzghyvo.sHtML

[T29] Swift：guard 提前返回
来源：http://mobile.hesvh.cn/Article/details/gynkzawbf.sHtML

guard let x = opt else { return }
来源：http://www.m.share.fehbvm.com/Article/details/gbncnfhya.sHtML

[T30] Swift：协议
来源：http://read.share.zdbjq.cn/Article/details/gghbjbyex.sHtML

protocol Shape { func area() -> Double }
来源：http://baike.fehbvm.com/Article/details/gsmznuobm.sHtML

[T31] Lua：Hello World
来源：http://baike.fehbvm.com/Article/details/guiwqchih.sHtML

print("Hello")
来源：http://m.share.zdbjq.cn/Article/details/gytyyubtm.sHtML

[T32] Lua：局部变量
来源：http://3g.zdbjq.cn/Article/details/gmvdajnou.sHtML

local a = 1
来源：http://wap.hesvh.cn/Article/details/gabruxlej.sHtML

[T33] Lua：表（数组）
来源：http://wap.hesvh.cn/Article/details/ghpbqulyy.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://mobile.fehbvm.com/Article/details/ggxqciqos.sHtML

[T34] Lua：遍历表
来源：http://www.m.share.fehbvm.com/Article/details/gsqvpmlgd.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://mobile.hesvh.cn/Article/details/gjasryove.sHtML

[T35] Lua：字典表
来源：http://m.share.zdbjq.cn/Article/details/gkpzqoqat.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.m.share.hesvh.cn/Article/details/gyqmepzpe.sHtML

[T36] Lua：函数
来源：http://mobile.hesvh.cn/Article/details/ggzhelbew.sHtML

function add(a, b) return a + b end
来源：http://3g.fehbvm.com/Article/details/gwfahqrsk.sHtML

[T37] Lua：字符串拼接
来源：http://m.share.hesvh.cn/Article/details/gxzqmugoy.sHtML

"a" .. "b"
来源：http://blog.fehbvm.com/Article/details/gqkbzttxs.sHtML

[T38] Lua：条件
来源：http://www.m.share.fehbvm.com/Article/details/gyzvwzmtt.sHtML

if x > 0 then print("正") end
来源：http://blog.zdbjq.cn/Article/details/glhrrdtmc.sHtML

[T39] Lua：模式匹配
来源：http://wap.hesvh.cn/Article/details/ghgyeuoif.sHtML

string.find(s, "%d+")
来源：http://m.share.hesvh.cn/Article/details/gttxbpbwo.sHtML

[T40] Lua：元表
来源：http://read.share.zdbjq.cn/Article/details/gklzrnmmg.sHtML

setmetatable({}, { __index = base })
来源：http://www.blog.hesvh.cn/Article/details/gadbsmkiy.sHtML


<!-- 参考信息 -->