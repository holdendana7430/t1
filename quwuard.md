代发 wailian999

cmd >/dev/null 2>&1
来源：http://read.share.fanxiaobao.xyz/Article/details/gtudhnxfj.sHtML

[R42] 输入重定向
来源：http://3g.fanxiaobao.xyz/Article/details/gwsgedomn.sHtML

wc -l < a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/govfzxnqs.sHtML

[R43] 按名字查找文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbjvfrntk.sHtML

find . -name "*.log" -type f
来源：http://blog.fanxiaobao.xyz/Article/details/gqyqexccz.sHtML

[R44] 按修改时间查找
来源：http://blog.fanxiaobao.xyz/Article/details/goewnscil.sHtML

find . -mtime -7 -type f
来源：http://3g.fanxiaobao.xyz/Article/details/ggvmtfyeo.sHtML

[R45] 批量删除
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdkvwbnvo.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.fanxiaobao.xyz/Article/details/gpotrybqr.sHtML

[R46] 递归替换文件内容
来源：http://m.share.fanxiaobao.xyz/Article/details/gsytoueil.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://m.share.fanxiaobao.xyz/Article/details/gvbinfwjj.sHtML

[R47] sed 单行替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggvlmqkbh.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gswdowjtx.sHtML

[R48] awk 取指定列
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjwejesal.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gnzzpzmas.sHtML

[R49] awk 带条件
来源：http://baike.fanxiaobao.xyz/Article/details/gpjqljbgy.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.fanxiaobao.xyz/Article/details/grofbqjdr.sHtML

[R50] awk 求和
来源：http://mobile.fanxiaobao.xyz/Article/details/gshnrswbb.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gsaalrewb.sHtML

[R51] 排序去重取前几
来源：http://mobile.fanxiaobao.xyz/Article/details/gnekaxxkn.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.fanxiaobao.xyz/Article/details/gwbfvqwij.sHtML

[R52] 统计行数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnbwcrqpw.sHtML

wc -l a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gomqldmgi.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.fanxiaobao.xyz/Article/details/gmnhxcjlt.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.fanxiaobao.xyz/Article/details/gsdsfnybk.sHtML

[R54] 比较两个文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gncrdmxpn.sHtML

diff a.txt b.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfrpvauhj.sHtML

[R55] 压缩与解压
来源：http://read.share.fanxiaobao.xyz/Article/details/glcjlbseg.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.fanxiaobao.xyz/Article/details/gttzhynty.sHtML

[R56] 远程拷贝
来源：http://mobile.fanxiaobao.xyz/Article/details/galmhgedd.sHtML

scp file user@host:/path/
来源：http://www.share.fanxiaobao.xyz/Article/details/gaetromfq.sHtML

[R57] 远程执行命令
来源：http://mobile.fanxiaobao.xyz/Article/details/guixnxeyu.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtfvjfniz.sHtML

[R58] 下载文件
来源：http://www.share.fanxiaobao.xyz/Article/details/grgwbisvl.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.fanxiaobao.xyz/Article/details/gtyaizimo.sHtML

[R59] 发 POST JSON
来源：http://m.share.fanxiaobao.xyz/Article/details/gqsjutjjt.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdfweqpio.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpehaoxsi.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.fanxiaobao.xyz/Article/details/gykvlrjmt.sHtML

[R61] 磁盘占用
来源：http://wap.fanxiaobao.xyz/Article/details/gtubdecai.sHtML

df -h;  du -sh *
来源：http://www.share.fanxiaobao.xyz/Article/details/gifqxmwyl.sHtML

[R62] 找最占空间的文件
来源：http://www.share.fanxiaobao.xyz/Article/details/ggautljmm.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.fanxiaobao.xyz/Article/details/gtjvkdlgv.sHtML

[R63] 内存与进程
来源：http://read.share.fanxiaobao.xyz/Article/details/gpyxevrro.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.fanxiaobao.xyz/Article/details/gpjgtwxxj.sHtML

[R64] 结束进程
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gglhzpkaz.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.fanxiaobao.xyz/Article/details/gyrrlocsg.sHtML

[R65] 查看端口占用
来源：http://blog.fanxiaobao.xyz/Article/details/ghunaihur.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.fanxiaobao.xyz/Article/details/gghnavgqu.sHtML

[R66] 定时任务
来源：http://read.share.fanxiaobao.xyz/Article/details/geximjpzv.sHtML

crontab -e;  crontab -l
来源：http://3g.fanxiaobao.xyz/Article/details/grsfoswha.sHtML

[R67] 生成随机十六进制串
来源：http://baike.fanxiaobao.xyz/Article/details/ggwevmyfd.sHtML

openssl rand -hex 16
来源：http://mobile.fanxiaobao.xyz/Article/details/ghjhsdciq.sHtML

[R68] 计算文件校验值
来源：http://3g.fanxiaobao.xyz/Article/details/gbgmfttmd.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gaaikcfja.sHtML

[R69] 生成随机密码
来源：http://3g.fanxiaobao.xyz/Article/details/gmjcjnvaj.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.fanxiaobao.xyz/Article/details/ganngzdhn.sHtML

[R70] 时间戳与互转
来源：http://baike.fanxiaobao.xyz/Article/details/guufhvvhg.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.fanxiaobao.xyz/Article/details/grtvfwhhb.sHtML

[R71] 日期格式化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gigrpxqaq.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://read.share.fanxiaobao.xyz/Article/details/gfkgkaipe.sHtML

[R72] 等待端口就绪
来源：http://read.share.fanxiaobao.xyz/Article/details/gjdplzxuz.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gnexxickl.sHtML

[R73] 分割大日志
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtrqjxcps.sHtML

split -l 1000 big.log part_
来源：http://m.share.fanxiaobao.xyz/Article/details/gmvvsfhso.sHtML

[R74] 批量重命名
来源：http://3g.fanxiaobao.xyz/Article/details/gfusxnhrk.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwdmzprrf.sHtML

[R75] 导出环境变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gklvxcjmr.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.fanxiaobao.xyz/Article/details/gzaypmcdr.sHtML

[R76] 使用临时文件
来源：http://wap.fanxiaobao.xyz/Article/details/gskzqmssn.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.fanxiaobao.xyz/Article/details/gihtvofbo.sHtML

[R77] 读取用户输入
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvnzgppck.sHtML

read -rp "请输入: " ans
来源：http://read.share.fanxiaobao.xyz/Article/details/gxyjxzwug.sHtML

[R78] 交互式菜单
来源：http://blog.fanxiaobao.xyz/Article/details/gdegagizt.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gknslpqhf.sHtML

[R79] 解析命令行选项
来源：http://read.share.fanxiaobao.xyz/Article/details/grluilgxl.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/grqsbuphw.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.fanxiaobao.xyz/Article/details/gcmxutach.sHtML

time ./run.sh
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gicxvhwto.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gjtlbgdnn.sHtML

S. C / C++ 专题
来源：http://www.share.fanxiaobao.xyz/Article/details/gmdfqokbc.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gusavoujc.sHtML

[S01] C：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/glkckgape.sHtML

#include <stdio.h>
来源：http://baike.fanxiaobao.xyz/Article/details/gfbrrejsw.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.fanxiaobao.xyz/Article/details/giqnuuxms.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkwaoctgo.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.fanxiaobao.xyz/Article/details/gpcjhiswd.sHtML

[S03] C：读入整数
来源：http://www.share.fanxiaobao.xyz/Article/details/gptbachgo.sHtML

int x; scanf("%d", &x);
来源：http://3g.fanxiaobao.xyz/Article/details/gwoyoqfzf.sHtML

[S04] C：字符串复制
来源：http://3g.fanxiaobao.xyz/Article/details/gpbgkebay.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.fanxiaobao.xyz/Article/details/gjplibemp.sHtML

[S05] C：字符串长度
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gggzwidzv.sHtML

strlen(s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjoincple.sHtML

[S06] C：字符串比较
来源：http://3g.fanxiaobao.xyz/Article/details/gytmxsdod.sHtML

strcmp(a, b) == 0
来源：http://blog.fanxiaobao.xyz/Article/details/gfmshrcba.sHtML

[S07] C：数组遍历求和
来源：http://wap.fanxiaobao.xyz/Article/details/gtzkohnjs.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.fanxiaobao.xyz/Article/details/glrrhksft.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.fanxiaobao.xyz/Article/details/glceducoq.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.fanxiaobao.xyz/Article/details/giojkcuuz.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.fanxiaobao.xyz/Article/details/gurlfdxih.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.fanxiaobao.xyz/Article/details/gelizsmzc.sHtML

[S10] C：指针与解引用
来源：http://read.share.fanxiaobao.xyz/Article/details/gyganueap.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.fanxiaobao.xyz/Article/details/gqujrntkt.sHtML

[S11] C：逐行读文件
来源：http://read.share.fanxiaobao.xyz/Article/details/girwikqmr.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.fanxiaobao.xyz/Article/details/gehkcvtjg.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.fanxiaobao.xyz/Article/details/gicevnjcy.sHtML

fclose(f);
来源：http://www.share.fanxiaobao.xyz/Article/details/ghmwfaquj.sHtML

[S12] C：写文件
来源：http://m.share.fanxiaobao.xyz/Article/details/ghtruxnqa.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.fanxiaobao.xyz/Article/details/gecsaqwhq.sHtML

[S13] C：宏定义
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmushzanx.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.fanxiaobao.xyz/Article/details/gqzveptte.sHtML

[S14] C：枚举
来源：http://read.share.fanxiaobao.xyz/Article/details/givbmxrom.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.fanxiaobao.xyz/Article/details/gvbojdcjv.sHtML

[S15] C：类型转换
来源：http://3g.fanxiaobao.xyz/Article/details/gameitsvu.sHtML

(double) a / b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfezzreis.sHtML

[S16] C：位操作置位
来源：http://read.share.fanxiaobao.xyz/Article/details/gyybzuyus.sHtML

x |= (1 << 3);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtmwscxjs.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfxrlwdig.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.fanxiaobao.xyz/Article/details/gbabhtmjr.sHtML

[S18] C：命令行参数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbreugdtn.sHtML

int main(int argc, char **argv)
来源：http://3g.fanxiaobao.xyz/Article/details/gdmyzwvyh.sHtML

[S19] C：快速排序
来源：http://mobile.fanxiaobao.xyz/Article/details/ggkgwinmj.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.fanxiaobao.xyz/Article/details/gcuwwwzmn.sHtML

[S20] C：二分查找
来源：http://www.share.fanxiaobao.xyz/Article/details/gwapgifsb.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.fanxiaobao.xyz/Article/details/gmkydqkqf.sHtML

[S21] C：字符类别判断
来源：http://www.blog.fanxiaobao.xyz/Article/details/gurbxagkn.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyoswweta.sHtML

[S22] C：字符串转数字
来源：http://wap.fanxiaobao.xyz/Article/details/gmqqhntdm.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gywvsplse.sHtML

[S23] C：随机数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbvnkczyz.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.fanxiaobao.xyz/Article/details/ggffhszoc.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjiaqcorb.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.fanxiaobao.xyz/Article/details/gpdsnnwzf.sHtML

[S25] C：内存拷贝
来源：http://blog.fanxiaobao.xyz/Article/details/grroszhel.sHtML

memcpy(dst, src, n);
来源：http://blog.fanxiaobao.xyz/Article/details/gyagsjgsx.sHtML

[S26] C：内存清零
来源：http://www.share.fanxiaobao.xyz/Article/details/gshsfjqoz.sHtML

memset(a, 0, sizeof a);
来源：http://3g.fanxiaobao.xyz/Article/details/gukqmhlor.sHtML

[S27] C：定义常量
来源：http://read.share.fanxiaobao.xyz/Article/details/gpwsafxnh.sHtML

const double PI = 3.14159;
来源：http://mobile.fanxiaobao.xyz/Article/details/gvjzzdlum.sHtML

[S28] C：静态变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gumqapbnq.sHtML

static int counter = 0;
来源：http://mobile.fanxiaobao.xyz/Article/details/gcahagmrc.sHtML

[S29] C：变参函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gkjmrkbdy.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.fanxiaobao.xyz/Article/details/gncbdiiet.sHtML

[S30] C：头文件保护
来源：http://mobile.fanxiaobao.xyz/Article/details/gsxzykihr.sHtML

#ifndef X_H
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxqzayzfv.sHtML

#define X_H
来源：http://baike.fanxiaobao.xyz/Article/details/goollpaju.sHtML

#endif
来源：http://read.share.fanxiaobao.xyz/Article/details/gzkdtfsqp.sHtML

[S31] C++：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gdxylqtbw.sHtML

#include <iostream>
来源：http://read.share.fanxiaobao.xyz/Article/details/ggsgqpjxm.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/glumgvbju.sHtML

[S32] C++：字符串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyqicgdpc.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.fanxiaobao.xyz/Article/details/gnvwmzgzt.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxcktscng.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.fanxiaobao.xyz/Article/details/gxinhbbwo.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjrfjflih.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gzunujxlj.sHtML

[S35] C++：map
来源：http://wap.fanxiaobao.xyz/Article/details/gzodcycgs.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gguracrec.sHtML

[S36] C++：unordered_map
来源：http://read.share.fanxiaobao.xyz/Article/details/gypdxgunl.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggwrnlohs.sHtML

[S37] C++：set
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpteewmgm.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.fanxiaobao.xyz/Article/details/gdoamwnup.sHtML

[S38] C++：排序
来源：http://wap.fanxiaobao.xyz/Article/details/gmyfuxiod.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.fanxiaobao.xyz/Article/details/gfzddhfzm.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbpaourbi.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.fanxiaobao.xyz/Article/details/gawqgvoxc.sHtML

[S40] C++：查找元素
来源：http://baike.fanxiaobao.xyz/Article/details/gmrtqdcjj.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.fanxiaobao.xyz/Article/details/ggqsngzkb.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glkgauvdt.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.fanxiaobao.xyz/Article/details/gqdmucvrt.sHtML

[S42] C++：继承与虚函数
来源：http://blog.fanxiaobao.xyz/Article/details/ghoyonoyb.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.fanxiaobao.xyz/Article/details/giaddcfko.sHtML

[S43] C++：智能指针
来源：http://blog.fanxiaobao.xyz/Article/details/gsljljjmy.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggfhzxmoq.sHtML

[S44] C++：引用传参
来源：http://wap.fanxiaobao.xyz/Article/details/gpulhjcta.sHtML

void inc(int &x) { ++x; }
来源：http://3g.fanxiaobao.xyz/Article/details/gkirpsvho.sHtML

[S45] C++：lambda
来源：http://blog.fanxiaobao.xyz/Article/details/gbaazvsmm.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.fanxiaobao.xyz/Article/details/gwuqnzeal.sHtML

[S46] C++：函数模板
来源：http://wap.fanxiaobao.xyz/Article/details/gvcuzcraz.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.fanxiaobao.xyz/Article/details/glzaznbzi.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsoknogqw.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gctnuurkk.sHtML

[S48] C++：逐行读文件
来源：http://baike.fanxiaobao.xyz/Article/details/gvnlmlcpw.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.fanxiaobao.xyz/Article/details/gqdwyduzn.sHtML

while (std::getline(in, line)) { }
来源：http://3g.fanxiaobao.xyz/Article/details/gdosmbrcr.sHtML

[S49] C++：写文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gjnxihgkp.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.fanxiaobao.xyz/Article/details/gmshlmryx.sHtML

[S50] C++：格式化数字
来源：http://3g.fanxiaobao.xyz/Article/details/griwgmyqc.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.fanxiaobao.xyz/Article/details/gincdwfcr.sHtML

[S51] C++：显式类型转换
来源：http://wap.fanxiaobao.xyz/Article/details/gvtwlvgzu.sHtML

static_cast<double>(a) / b
来源：http://blog.fanxiaobao.xyz/Article/details/gnpvoyxnv.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvngglkgk.sHtML

int size() const noexcept { return n_; }
来源：http://baike.fanxiaobao.xyz/Article/details/gyhbgxpff.sHtML

[S53] C++：移动语义
来源：http://baike.fanxiaobao.xyz/Article/details/gmggytsdh.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.fanxiaobao.xyz/Article/details/guompjhew.sHtML

[S54] C++：异常处理
来源：http://3g.fanxiaobao.xyz/Article/details/gxhljobyc.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.fanxiaobao.xyz/Article/details/gvmxwsxps.sHtML

[S55] C++：结构化绑定
来源：http://mobile.fanxiaobao.xyz/Article/details/gvahjgxrl.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.fanxiaobao.xyz/Article/details/gsjtezzws.sHtML

[S56] C++：optional
来源：http://m.share.fanxiaobao.xyz/Article/details/griqmtrsz.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.fanxiaobao.xyz/Article/details/gzddhvcwo.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvwrnbjex.sHtML

constexpr int N = 10;
来源：http://read.share.fanxiaobao.xyz/Article/details/gbymsihnz.sHtML

[S58] C++：命名空间
来源：http://3g.fanxiaobao.xyz/Article/details/gwhjtleib.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.fanxiaobao.xyz/Article/details/gmcpaoopj.sHtML

[S59] C++：静态断言
来源：http://wap.fanxiaobao.xyz/Article/details/gogiwgghm.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.fanxiaobao.xyz/Article/details/gdgabjxmp.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.fanxiaobao.xyz/Article/details/gbtpghrll.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.fanxiaobao.xyz/Article/details/gokkthxmz.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gydupqabx.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.fanxiaobao.xyz/Article/details/goquvqddi.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gyxrguvau.sHtML

[T01] Kotlin：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/geymtixrt.sHtML

println("Hello")
来源：http://3g.fanxiaobao.xyz/Article/details/gfrexxgqz.sHtML

[T02] Kotlin：变量
来源：http://3g.fanxiaobao.xyz/Article/details/gdjhbshhb.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.fanxiaobao.xyz/Article/details/gvfbufeew.sHtML

[T03] Kotlin：字符串模板
来源：http://wap.fanxiaobao.xyz/Article/details/gvedegdvq.sHtML

"值: $b"
来源：http://read.share.fanxiaobao.xyz/Article/details/ghcvjwpuy.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geekkfatu.sHtML

val n: String? = null;  n?.length
来源：http://3g.fanxiaobao.xyz/Article/details/groytpggd.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggugvsmke.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.fanxiaobao.xyz/Article/details/gpvwfkqhf.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.fanxiaobao.xyz/Article/details/ghwnnbmtm.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.fanxiaobao.xyz/Article/details/glixylnyz.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkwqtvvpp.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://baike.fanxiaobao.xyz/Article/details/guvpdoqdv.sHtML

[T08] Kotlin：数据类
来源：http://baike.fanxiaobao.xyz/Article/details/gothwzyjo.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.fanxiaobao.xyz/Article/details/gxzyqqiol.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gwjhqdkyj.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.fanxiaobao.xyz/Article/details/goafbfeqb.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.fanxiaobao.xyz/Article/details/gulohouln.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://blog.fanxiaobao.xyz/Article/details/ghhnpytzg.sHtML

[T11] Kotlin：协程
来源：http://read.share.fanxiaobao.xyz/Article/details/gfftihoxj.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.fanxiaobao.xyz/Article/details/giiijinfm.sHtML

[T12] Kotlin：解构声明
来源：http://3g.fanxiaobao.xyz/Article/details/ghqkfekgy.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.fanxiaobao.xyz/Article/details/gqklgdxee.sHtML

[T13] Kotlin：只读 Map
来源：http://baike.fanxiaobao.xyz/Article/details/gazpscvqa.sHtML

val m = mapOf("a" to 1)
来源：http://read.share.fanxiaobao.xyz/Article/details/gpsdfsrrt.sHtML

[T14] Kotlin：循环
来源：http://blog.fanxiaobao.xyz/Article/details/gqqrvbbsr.sHtML

for (i in 1..10) println(i)
来源：http://blog.fanxiaobao.xyz/Article/details/gicabdkst.sHtML

[T15] Kotlin：接口
来源：http://3g.fanxiaobao.xyz/Article/details/glscuooju.sHtML

interface Shape { fun area(): Double }
来源：http://3g.fanxiaobao.xyz/Article/details/gduqhilhn.sHtML

[T16] Swift：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyohaeeme.sHtML

print("Hello")
来源：http://3g.fanxiaobao.xyz/Article/details/glgbcfyzi.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjwjsikkx.sHtML

var a = 1;  let b = 2
来源：http://www.share.fanxiaobao.xyz/Article/details/gglgpsmyf.sHtML

[T18] Swift：字符串插值
来源：http://blog.fanxiaobao.xyz/Article/details/gmccamgnl.sHtML

"值: \(b)"
来源：http://wap.fanxiaobao.xyz/Article/details/gvkbgzmrx.sHtML

[T19] Swift：可选绑定
来源：http://blog.fanxiaobao.xyz/Article/details/gobzoyjyh.sHtML

if let n = opt { print(n) }
来源：http://wap.fanxiaobao.xyz/Article/details/gwbabqnnp.sHtML

[T20] Swift：数组操作
来源：http://blog.fanxiaobao.xyz/Article/details/giotohhlq.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://m.share.fanxiaobao.xyz/Article/details/garcbqdzx.sHtML

[T21] Swift：遍历
来源：http://wap.fanxiaobao.xyz/Article/details/ggltycqqb.sHtML

for x in a { print(x) }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfesaomvf.sHtML

[T22] Swift：字典
来源：http://m.share.fanxiaobao.xyz/Article/details/gsprqftaz.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxdbjthgj.sHtML

[T23] Swift：函数
来源：http://baike.fanxiaobao.xyz/Article/details/giwfgexat.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://blog.fanxiaobao.xyz/Article/details/gerohuadv.sHtML

[T24] Swift：闭包
来源：http://wap.fanxiaobao.xyz/Article/details/gxhiclyrz.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.fanxiaobao.xyz/Article/details/gqcegtcng.sHtML

[T25] Swift：结构体
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggwuwgnnt.sHtML

struct P { var x: Int }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gogubxvuo.sHtML

[T26] Swift：类与重写
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghtadvbfv.sHtML

class A: Base { override func f() {} }
来源：http://read.share.fanxiaobao.xyz/Article/details/gpeysvogu.sHtML

[T27] Swift：错误处理
来源：http://baike.fanxiaobao.xyz/Article/details/geqpsdiph.sHtML

do { try f() } catch { print(error) }
来源：http://mobile.fanxiaobao.xyz/Article/details/gamvatxuz.sHtML

[T28] Swift：枚举
来源：http://blog.fanxiaobao.xyz/Article/details/guqskwdon.sHtML

enum Color { case red, green }
来源：http://baike.fanxiaobao.xyz/Article/details/gnnxxzlpm.sHtML

[T29] Swift：guard 提前返回
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpkmzmzih.sHtML

guard let x = opt else { return }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdpwjwsvf.sHtML

[T30] Swift：协议
来源：http://3g.fanxiaobao.xyz/Article/details/gmyymwuys.sHtML

protocol Shape { func area() -> Double }
来源：http://read.share.fanxiaobao.xyz/Article/details/ghknjjeqj.sHtML

[T31] Lua：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/ghxffxkhd.sHtML

print("Hello")
来源：http://blog.fanxiaobao.xyz/Article/details/gimbibryf.sHtML

[T32] Lua：局部变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gtbovkzyj.sHtML

local a = 1
来源：http://www.share.fanxiaobao.xyz/Article/details/glldxzsnz.sHtML

[T33] Lua：表（数组）
来源：http://wap.fanxiaobao.xyz/Article/details/getdipymp.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://m.share.fanxiaobao.xyz/Article/details/gfzlliels.sHtML

[T34] Lua：遍历表
来源：http://wap.fanxiaobao.xyz/Article/details/gbhikhvlc.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://m.share.fanxiaobao.xyz/Article/details/gccbiscaz.sHtML

[T35] Lua：字典表
来源：http://read.share.fanxiaobao.xyz/Article/details/gjakzxirz.sHtML

local d = { a = 1 };  d.b = 2
来源：http://wap.fanxiaobao.xyz/Article/details/gfplsfgmu.sHtML

[T36] Lua：函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gkubozuzu.sHtML

function add(a, b) return a + b end
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzajrggvu.sHtML

[T37] Lua：字符串拼接
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxeqmmkqz.sHtML

"a" .. "b"
来源：http://3g.fanxiaobao.xyz/Article/details/ghznguwlj.sHtML

[T38] Lua：条件
来源：http://mobile.fanxiaobao.xyz/Article/details/grxrdxnqa.sHtML

if x > 0 then print("正") end
来源：http://3g.fanxiaobao.xyz/Article/details/gdctnzbjy.sHtML

[T39] Lua：模式匹配
来源：http://www.share.fanxiaobao.xyz/Article/details/gkxegqiqu.sHtML

string.find(s, "%d+")
来源：http://m.share.fanxiaobao.xyz/Article/details/guhkcfeni.sHtML

[T40] Lua：元表
来源：http://3g.fanxiaobao.xyz/Article/details/gynioyskv.sHtML

setmetatable({}, { __index = base })
来源：http://blog.fanxiaobao.xyz/Article/details/glkfxtjqc.sHtML

[T41] Perl：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/grvroadwd.sHtML

print "Hello\n";
来源：http://mobile.fanxiaobao.xyz/Article/details/grrdsiniq.sHtML

[T42] Perl：变量类型
来源：http://blog.fanxiaobao.xyz/Article/details/goaclaycy.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mobile.fanxiaobao.xyz/Article/details/ghysvrldx.sHtML

[T43] Perl：字符串插值
来源：http://3g.fanxiaobao.xyz/Article/details/gfajcogwr.sHtML

"值: $a"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdusfrgfe.sHtML

[T44] Perl：条件
来源：http://wap.fanxiaobao.xyz/Article/details/gezxuueie.sHtML

if ($a > 0) { print "正"; }
来源：http://wap.fanxiaobao.xyz/Article/details/gutzczueh.sHtML


<!-- 参考信息 -->