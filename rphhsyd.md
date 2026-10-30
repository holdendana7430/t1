代发 wailian999

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.hesvh.cn/Article/details/gwtmkvjlp.sHtML

[R36] 并发执行多个任务
来源：http://read.share.fehbvm.com/Article/details/gcistireq.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.hesvh.cn/Article/details/grluutpbq.sHtML

[R37] 把输出赋给变量
来源：http://read.share.fehbvm.com/Article/details/gzrckdfkr.sHtML

files=$(ls -1)
来源：http://www.share.zdbjq.cn/Article/details/gviwmckyi.sHtML

[R38] 管道串联
来源：http://wap.zdbjq.cn/Article/details/goihkmqgx.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.zdbjq.cn/Article/details/gxdmkheqj.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.hesvh.cn/Article/details/gnljxzkuf.sHtML

cmd > out.log 2>&1
来源：http://read.share.zdbjq.cn/Article/details/grgmvtdvn.sHtML

[R40] 追加写日志
来源：http://wap.zdbjq.cn/Article/details/gtwvkozss.sHtML

echo "log" >> out.log
来源：http://mobile.fehbvm.com/Article/details/gnahchtir.sHtML

[R41] 丢弃输出
来源：http://wap.hesvh.cn/Article/details/gtbrmtlre.sHtML

cmd >/dev/null 2>&1
来源：http://3g.hesvh.cn/Article/details/gcynnjwic.sHtML

[R42] 输入重定向
来源：http://mobile.fehbvm.com/Article/details/gqqajplvc.sHtML

wc -l < a.txt
来源：http://3g.fehbvm.com/Article/details/gqpeifwps.sHtML

[R43] 按名字查找文件
来源：http://wap.hesvh.cn/Article/details/galkshczq.sHtML

find . -name "*.log" -type f
来源：http://3g.zdbjq.cn/Article/details/gmkqxipud.sHtML

[R44] 按修改时间查找
来源：http://read.share.hesvh.cn/Article/details/gfqieyaih.sHtML

find . -mtime -7 -type f
来源：http://3g.hesvh.cn/Article/details/gkumaagzn.sHtML

[R45] 批量删除
来源：http://mobile.zdbjq.cn/Article/details/gteozrkvb.sHtML

find . -name "*.tmp" -delete
来源：http://blog.hesvh.cn/Article/details/glyskjsop.sHtML

[R46] 递归替换文件内容
来源：http://m.share.zdbjq.cn/Article/details/goeduwvgo.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.hesvh.cn/Article/details/ghtbjvvxb.sHtML

[R47] sed 单行替换
来源：http://mobile.hesvh.cn/Article/details/gbnvkeyxh.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.hesvh.cn/Article/details/geqetynwz.sHtML

[R48] awk 取指定列
来源：http://mobile.hesvh.cn/Article/details/grcmwalud.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.fehbvm.com/Article/details/gzxvessee.sHtML

[R49] awk 带条件
来源：http://wap.zdbjq.cn/Article/details/gihvlfywz.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.fehbvm.com/Article/details/gqxijejyf.sHtML

[R50] awk 求和
来源：http://3g.hesvh.cn/Article/details/gwxhduojq.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.fehbvm.com/Article/details/gsucbrvml.sHtML

[R51] 排序去重取前几
来源：http://wap.hesvh.cn/Article/details/gkcuedvbl.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.hesvh.cn/Article/details/ggsgjfylv.sHtML

[R52] 统计行数
来源：http://read.share.zdbjq.cn/Article/details/ghleasfyv.sHtML

wc -l a.txt
来源：http://blog.hesvh.cn/Article/details/gjbtfhjfr.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.zdbjq.cn/Article/details/glbygmpsp.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.hesvh.cn/Article/details/gwzszqfvx.sHtML

[R54] 比较两个文件
来源：http://3g.fehbvm.com/Article/details/gttepyazh.sHtML

diff a.txt b.txt
来源：http://read.share.zdbjq.cn/Article/details/gecghgmny.sHtML

[R55] 压缩与解压
来源：http://www.m.share.hesvh.cn/Article/details/gfaeocsqk.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.zdbjq.cn/Article/details/grblmgyrl.sHtML

[R56] 远程拷贝
来源：http://mobile.zdbjq.cn/Article/details/gsqmhsbhi.sHtML

scp file user@host:/path/
来源：http://blog.fehbvm.com/Article/details/gigmudwgf.sHtML

[R57] 远程执行命令
来源：http://www.m.share.fehbvm.com/Article/details/gjhbpdfju.sHtML

ssh user@host 'uptime'
来源：http://www.share.fehbvm.com/Article/details/gnxxjmuog.sHtML

[R58] 下载文件
来源：http://3g.zdbjq.cn/Article/details/gpzlpulxl.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.fehbvm.com/Article/details/gfllmfrvp.sHtML

[R59] 发 POST JSON
来源：http://blog.fehbvm.com/Article/details/glnxeoxdm.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.fehbvm.com/Article/details/gzsperjyq.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.fehbvm.com/Article/details/gsjxhltik.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.fehbvm.com/Article/details/gnejcptlh.sHtML

[R61] 磁盘占用
来源：http://mobile.hesvh.cn/Article/details/gwhrogdkm.sHtML

df -h;  du -sh *
来源：http://m.share.hesvh.cn/Article/details/gsdturqns.sHtML

[R62] 找最占空间的文件
来源：http://wap.fehbvm.com/Article/details/gjcvfqoht.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.zdbjq.cn/Article/details/gazepghqx.sHtML

[R63] 内存与进程
来源：http://m.share.hesvh.cn/Article/details/gmrfjzgkv.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.zdbjq.cn/Article/details/gmorlitvk.sHtML

[R64] 结束进程
来源：http://www.m.share.hesvh.cn/Article/details/gkuaabvou.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.zdbjq.cn/Article/details/goxztuedc.sHtML

[R65] 查看端口占用
来源：http://www.share.fehbvm.com/Article/details/guirylrmp.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.hesvh.cn/Article/details/gslmsianv.sHtML

[R66] 定时任务
来源：http://www.m.share.hesvh.cn/Article/details/gjoroatbk.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.fehbvm.com/Article/details/gqnmisunk.sHtML

[R67] 生成随机十六进制串
来源：http://3g.zdbjq.cn/Article/details/ghqovbuic.sHtML

openssl rand -hex 16
来源：http://wap.zdbjq.cn/Article/details/gjefioane.sHtML

[R68] 计算文件校验值
来源：http://www.share.hesvh.cn/Article/details/gwcnlgsif.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.zdbjq.cn/Article/details/gvajguvfw.sHtML

[R69] 生成随机密码
来源：http://www.blog.fehbvm.com/Article/details/gaqyfrzfg.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.hesvh.cn/Article/details/ghpjkhpmt.sHtML

[R70] 时间戳与互转
来源：http://wap.hesvh.cn/Article/details/gkjtxkuiw.sHtML

date +%s;  date -d @1700000000
来源：http://blog.fehbvm.com/Article/details/gbicuxkrb.sHtML

[R71] 日期格式化
来源：http://m.share.hesvh.cn/Article/details/gdiewxkvw.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.zdbjq.cn/Article/details/gfdecxwgw.sHtML

[R72] 等待端口就绪
来源：http://3g.zdbjq.cn/Article/details/ggohwfuzo.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.fehbvm.com/Article/details/gxdteustu.sHtML

[R73] 分割大日志
来源：http://www.share.zdbjq.cn/Article/details/gnwnlwusj.sHtML

split -l 1000 big.log part_
来源：http://3g.zdbjq.cn/Article/details/gkujaxblc.sHtML

[R74] 批量重命名
来源：http://www.share.zdbjq.cn/Article/details/gwerhenxh.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.zdbjq.cn/Article/details/gyrbfgsmq.sHtML

[R75] 导出环境变量
来源：http://baike.hesvh.cn/Article/details/gdcejlfma.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.hesvh.cn/Article/details/gksydqeym.sHtML

[R76] 使用临时文件
来源：http://www.blog.fehbvm.com/Article/details/gtqqtabuy.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.hesvh.cn/Article/details/gmpmzgruv.sHtML

[R77] 读取用户输入
来源：http://3g.fehbvm.com/Article/details/gzhfvyseh.sHtML

read -rp "请输入: " ans
来源：http://m.share.fehbvm.com/Article/details/gitqupjys.sHtML

[R78] 交互式菜单
来源：http://www.share.hesvh.cn/Article/details/gcfzqhqez.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.hesvh.cn/Article/details/genhfsofs.sHtML

[R79] 解析命令行选项
来源：http://m.share.zdbjq.cn/Article/details/gdzlajlvc.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.fehbvm.com/Article/details/gucynnntq.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.fehbvm.com/Article/details/gawtkvdfp.sHtML

time ./run.sh
来源：http://mobile.fehbvm.com/Article/details/gausfhhgw.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gffbaxgkc.sHtML

S. C / C++ 专题
来源：http://read.share.hesvh.cn/Article/details/grrjwbmsu.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gnkemlnwg.sHtML

[S01] C：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/gsnvuvfyy.sHtML

#include <stdio.h>
来源：http://www.blog.fehbvm.com/Article/details/gzwpjmxoi.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.hesvh.cn/Article/details/gcmmcgerw.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.fehbvm.com/Article/details/gcuuwvfhf.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.hesvh.cn/Article/details/grkkmnhpf.sHtML

[S03] C：读入整数
来源：http://www.blog.fehbvm.com/Article/details/ghcgccmyv.sHtML

int x; scanf("%d", &x);
来源：http://mobile.zdbjq.cn/Article/details/gszklvjob.sHtML

[S04] C：字符串复制
来源：http://3g.hesvh.cn/Article/details/gnrsjbcnf.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.fehbvm.com/Article/details/gescshcad.sHtML

[S05] C：字符串长度
来源：http://read.share.fehbvm.com/Article/details/gzeuexdby.sHtML

strlen(s)
来源：http://www.blog.zdbjq.cn/Article/details/gdlnkbook.sHtML

[S06] C：字符串比较
来源：http://baike.zdbjq.cn/Article/details/gevytnazu.sHtML

strcmp(a, b) == 0
来源：http://3g.fehbvm.com/Article/details/gfvvuqkdf.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.zdbjq.cn/Article/details/gkjclobpd.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.fehbvm.com/Article/details/gvpwjluwb.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.fehbvm.com/Article/details/gvcurbwcv.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.hesvh.cn/Article/details/gvsndhczr.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.zdbjq.cn/Article/details/gzvpdguic.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.hesvh.cn/Article/details/gkvdmgxrh.sHtML

[S10] C：指针与解引用
来源：http://www.share.fehbvm.com/Article/details/glzaqahca.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.hesvh.cn/Article/details/gfmhkmebu.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.fehbvm.com/Article/details/gjjqfkbgx.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.zdbjq.cn/Article/details/gckwhsfqi.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.hesvh.cn/Article/details/gernlhkgq.sHtML

fclose(f);
来源：http://www.share.fehbvm.com/Article/details/gfgcxgkxq.sHtML

[S12] C：写文件
来源：http://read.share.hesvh.cn/Article/details/gbbtjtutc.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.zdbjq.cn/Article/details/ggxlvqoxn.sHtML

[S13] C：宏定义
来源：http://3g.zdbjq.cn/Article/details/ghwsypkev.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.hesvh.cn/Article/details/gripsecli.sHtML

[S14] C：枚举
来源：http://blog.fehbvm.com/Article/details/gkeeilcah.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.fehbvm.com/Article/details/gwwrujrzh.sHtML

[S15] C：类型转换
来源：http://3g.hesvh.cn/Article/details/gesswhdyk.sHtML

(double) a / b
来源：http://wap.hesvh.cn/Article/details/gfibxdlel.sHtML

[S16] C：位操作置位
来源：http://read.share.zdbjq.cn/Article/details/gqfnnurij.sHtML

x |= (1 << 3);
来源：http://wap.zdbjq.cn/Article/details/gloyfppyr.sHtML

[S17] C：安全拼接字符串
来源：http://3g.hesvh.cn/Article/details/gipvbpexo.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.zdbjq.cn/Article/details/grhwkftas.sHtML

[S18] C：命令行参数
来源：http://blog.fehbvm.com/Article/details/ghryxecbl.sHtML

int main(int argc, char **argv)
来源：http://m.share.zdbjq.cn/Article/details/gkaxmdgln.sHtML

[S19] C：快速排序
来源：http://mobile.fehbvm.com/Article/details/gyfbkbpmz.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.hesvh.cn/Article/details/gtxrpwhgb.sHtML

[S20] C：二分查找
来源：http://www.blog.hesvh.cn/Article/details/gddvznhqz.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.fehbvm.com/Article/details/grrktdgla.sHtML

[S21] C：字符类别判断
来源：http://wap.fehbvm.com/Article/details/ghxblrnjq.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.fehbvm.com/Article/details/gdgpsseqr.sHtML

[S22] C：字符串转数字
来源：http://wap.fehbvm.com/Article/details/gvxpyhyho.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.zdbjq.cn/Article/details/grfkvvvmt.sHtML

[S23] C：随机数
来源：http://www.m.share.fehbvm.com/Article/details/gdmtdpndz.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.fehbvm.com/Article/details/gtemvrnur.sHtML

[S24] C：获取本地时间
来源：http://baike.zdbjq.cn/Article/details/gzhnkaevr.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.zdbjq.cn/Article/details/gvxvsrmeo.sHtML

[S25] C：内存拷贝
来源：http://baike.zdbjq.cn/Article/details/gqtrxijey.sHtML

memcpy(dst, src, n);
来源：http://m.share.fehbvm.com/Article/details/gmftqprwa.sHtML

[S26] C：内存清零
来源：http://www.share.zdbjq.cn/Article/details/gflagzjuy.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.fehbvm.com/Article/details/gtevyhtwa.sHtML

[S27] C：定义常量
来源：http://blog.zdbjq.cn/Article/details/grrxpckoi.sHtML

const double PI = 3.14159;
来源：http://www.m.share.fehbvm.com/Article/details/gtjjlxaol.sHtML

[S28] C：静态变量
来源：http://www.blog.fehbvm.com/Article/details/gyozwutgq.sHtML

static int counter = 0;
来源：http://3g.fehbvm.com/Article/details/gsmcarrij.sHtML

[S29] C：变参函数
来源：http://mobile.zdbjq.cn/Article/details/gowmpagfu.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.fehbvm.com/Article/details/gbbofxdff.sHtML

[S30] C：头文件保护
来源：http://read.share.fehbvm.com/Article/details/gnpfdlhhs.sHtML

#ifndef X_H
来源：http://www.m.share.zdbjq.cn/Article/details/gfjxhanoo.sHtML

#define X_H
来源：http://3g.fehbvm.com/Article/details/gxeccupow.sHtML

#endif
来源：http://read.share.fehbvm.com/Article/details/gutnaofjf.sHtML

[S31] C++：Hello World
来源：http://wap.hesvh.cn/Article/details/gvkegjgox.sHtML

#include <iostream>
来源：http://mobile.zdbjq.cn/Article/details/gdjpeadmf.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.fehbvm.com/Article/details/gikspfjwt.sHtML

[S32] C++：字符串
来源：http://wap.zdbjq.cn/Article/details/gwstctekw.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.zdbjq.cn/Article/details/gyhumvbao.sHtML

[S33] C++：vector 增删
来源：http://www.share.fehbvm.com/Article/details/gjmqswsgj.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.fehbvm.com/Article/details/gkqamezdx.sHtML

[S34] C++：遍历 vector
来源：http://mobile.fehbvm.com/Article/details/gffrzhfye.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.hesvh.cn/Article/details/gbpcsidxn.sHtML

[S35] C++：map
来源：http://www.share.hesvh.cn/Article/details/gsrqfzwwi.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.zdbjq.cn/Article/details/gufdfdzps.sHtML

[S36] C++：unordered_map
来源：http://baike.hesvh.cn/Article/details/gptfawwob.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.hesvh.cn/Article/details/gqzcfzvfn.sHtML

[S37] C++：set
来源：http://www.blog.fehbvm.com/Article/details/gbyylvixp.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.hesvh.cn/Article/details/gdkljaeod.sHtML

[S38] C++：排序
来源：http://m.share.hesvh.cn/Article/details/gwwjontpb.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.zdbjq.cn/Article/details/gwgkcdity.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.fehbvm.com/Article/details/gyveyveld.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.fehbvm.com/Article/details/gfaeqmdgf.sHtML

[S40] C++：查找元素
来源：http://mobile.fehbvm.com/Article/details/gcrokqpgl.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.hesvh.cn/Article/details/gcjyhouyz.sHtML

[S41] C++：类与构造函数
来源：http://wap.fehbvm.com/Article/details/gyaehuyvx.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.fehbvm.com/Article/details/gzhlewiyj.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.hesvh.cn/Article/details/gzxttwpdp.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.fehbvm.com/Article/details/gfxjobzon.sHtML

[S43] C++：智能指针
来源：http://baike.fehbvm.com/Article/details/gyahndkil.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.fehbvm.com/Article/details/giqpnpoqm.sHtML

[S44] C++：引用传参
来源：http://blog.hesvh.cn/Article/details/gcmiosvgd.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.zdbjq.cn/Article/details/ghwmqzokn.sHtML

[S45] C++：lambda
来源：http://m.share.hesvh.cn/Article/details/gvhwhdztb.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.hesvh.cn/Article/details/gzpqfuzqm.sHtML

[S46] C++：函数模板
来源：http://blog.fehbvm.com/Article/details/gelamurcu.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.zdbjq.cn/Article/details/gwgnxbunw.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.zdbjq.cn/Article/details/gfwjnbnpj.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.zdbjq.cn/Article/details/gqcdnqngz.sHtML

[S48] C++：逐行读文件
来源：http://3g.hesvh.cn/Article/details/gqldrelkp.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.zdbjq.cn/Article/details/gqreobaoi.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.fehbvm.com/Article/details/gaxdsytiu.sHtML

[S49] C++：写文件
来源：http://3g.zdbjq.cn/Article/details/gdwstiosp.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.zdbjq.cn/Article/details/grinmcute.sHtML

[S50] C++：格式化数字
来源：http://baike.zdbjq.cn/Article/details/gerhwyisu.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.hesvh.cn/Article/details/gazkdxajv.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.hesvh.cn/Article/details/ggsdhglfp.sHtML

static_cast<double>(a) / b
来源：http://mobile.hesvh.cn/Article/details/gabzgbkvs.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.hesvh.cn/Article/details/gngregcah.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.hesvh.cn/Article/details/gogxatyth.sHtML

[S53] C++：移动语义
来源：http://www.share.hesvh.cn/Article/details/gpmzdfish.sHtML

std::vector<int> w = std::move(v);
来源：http://www.blog.zdbjq.cn/Article/details/gnpvsclcv.sHtML

[S54] C++：异常处理
来源：http://read.share.hesvh.cn/Article/details/gjafvvxxa.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.hesvh.cn/Article/details/guyzefaki.sHtML

[S55] C++：结构化绑定
来源：http://3g.zdbjq.cn/Article/details/gkupmjpro.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.hesvh.cn/Article/details/gqvschjip.sHtML

[S56] C++：optional
来源：http://www.m.share.hesvh.cn/Article/details/gputfqilw.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.fehbvm.com/Article/details/gweruwqez.sHtML

[S57] C++：编译期常量
来源：http://mobile.fehbvm.com/Article/details/gtgssfwlc.sHtML

constexpr int N = 10;
来源：http://wap.fehbvm.com/Article/details/gwemwteje.sHtML

[S58] C++：命名空间
来源：http://3g.zdbjq.cn/Article/details/gmgnrvqkw.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.zdbjq.cn/Article/details/giiyjtovl.sHtML

[S59] C++：静态断言
来源：http://3g.fehbvm.com/Article/details/gqcctrels.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.hesvh.cn/Article/details/gepnescdl.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.zdbjq.cn/Article/details/gpyyeilpk.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.hesvh.cn/Article/details/gzsvgwwbr.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gamyzqgxw.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.fehbvm.com/Article/details/gwahiyppj.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/giekqtrbc.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gtzcvhzad.sHtML

println("Hello")
来源：http://www.share.zdbjq.cn/Article/details/gpvzytuew.sHtML

[T02] Kotlin：变量
来源：http://m.share.hesvh.cn/Article/details/godadiljk.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.fehbvm.com/Article/details/gmjudayuc.sHtML

[T03] Kotlin：字符串模板
来源：http://wap.hesvh.cn/Article/details/gebtjgulj.sHtML

"值: $b"
来源：http://baike.hesvh.cn/Article/details/gmoljmyop.sHtML

[T04] Kotlin：空安全
来源：http://3g.zdbjq.cn/Article/details/gghsbtgxy.sHtML

val n: String? = null;  n?.length
来源：http://www.m.share.fehbvm.com/Article/details/guuonrzzn.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.hesvh.cn/Article/details/gllfkhtbd.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.zdbjq.cn/Article/details/gaxtspblv.sHtML

[T06] Kotlin：集合映射
来源：http://wap.hesvh.cn/Article/details/gmywbeczw.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://mobile.fehbvm.com/Article/details/gvpbquzun.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.zdbjq.cn/Article/details/gofriuhbn.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.fehbvm.com/Article/details/gysttjlzo.sHtML

[T08] Kotlin：数据类
来源：http://baike.zdbjq.cn/Article/details/gkkmyftxc.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.zdbjq.cn/Article/details/gfeczqblo.sHtML

[T09] Kotlin：扩展函数
来源：http://blog.fehbvm.com/Article/details/gagimbqsz.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.zdbjq.cn/Article/details/ggjrozmcf.sHtML

[T10] Kotlin：默认参数
来源：http://blog.zdbjq.cn/Article/details/geabniqqd.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.fehbvm.com/Article/details/ghbtuhyez.sHtML

[T11] Kotlin：协程
来源：http://www.m.share.zdbjq.cn/Article/details/gytezmsfc.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.hesvh.cn/Article/details/gnnvisywz.sHtML

[T12] Kotlin：解构声明
来源：http://wap.fehbvm.com/Article/details/gbfpllvzx.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.zdbjq.cn/Article/details/gpacyinaz.sHtML

[T13] Kotlin：只读 Map
来源：http://m.share.zdbjq.cn/Article/details/gppvwdhzp.sHtML

val m = mapOf("a" to 1)
来源：http://wap.zdbjq.cn/Article/details/gbyqlxsee.sHtML

[T14] Kotlin：循环
来源：http://www.share.hesvh.cn/Article/details/gzqhjciat.sHtML

for (i in 1..10) println(i)
来源：http://baike.hesvh.cn/Article/details/gacvuqtvq.sHtML

[T15] Kotlin：接口
来源：http://blog.zdbjq.cn/Article/details/gepcmqxxv.sHtML

interface Shape { fun area(): Double }
来源：http://wap.fehbvm.com/Article/details/gztpbpceq.sHtML

[T16] Swift：Hello World
来源：http://read.share.hesvh.cn/Article/details/gxzkluccq.sHtML

print("Hello")
来源：http://www.blog.fehbvm.com/Article/details/gprptzlqq.sHtML

[T17] Swift：变量与常量
来源：http://wap.hesvh.cn/Article/details/gufqpkfcu.sHtML

var a = 1;  let b = 2
来源：http://wap.hesvh.cn/Article/details/gfjrrsjyb.sHtML

[T18] Swift：字符串插值
来源：http://blog.fehbvm.com/Article/details/ghjvfdvrh.sHtML

"值: \(b)"
来源：http://blog.zdbjq.cn/Article/details/gerzypfou.sHtML

[T19] Swift：可选绑定
来源：http://baike.fehbvm.com/Article/details/grodtuzki.sHtML

if let n = opt { print(n) }
来源：http://www.share.zdbjq.cn/Article/details/gjcyqscqe.sHtML

[T20] Swift：数组操作
来源：http://mobile.zdbjq.cn/Article/details/gqawtwzzm.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://baike.zdbjq.cn/Article/details/ggkyqkixv.sHtML

[T21] Swift：遍历
来源：http://www.m.share.zdbjq.cn/Article/details/gqdydscns.sHtML

for x in a { print(x) }
来源：http://blog.fehbvm.com/Article/details/gvglwmrkp.sHtML

[T22] Swift：字典
来源：http://wap.zdbjq.cn/Article/details/gqiybebmj.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.share.zdbjq.cn/Article/details/gmskhgvrh.sHtML

[T23] Swift：函数
来源：http://wap.fehbvm.com/Article/details/gheahoapi.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://3g.hesvh.cn/Article/details/gzezbcuvd.sHtML

[T24] Swift：闭包
来源：http://www.m.share.hesvh.cn/Article/details/gvtrevmsy.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://3g.hesvh.cn/Article/details/gcyxelzjl.sHtML

[T25] Swift：结构体
来源：http://www.share.zdbjq.cn/Article/details/glsmruejq.sHtML

struct P { var x: Int }
来源：http://wap.hesvh.cn/Article/details/ggwvnjklg.sHtML

[T26] Swift：类与重写
来源：http://www.share.fehbvm.com/Article/details/gcxksyatu.sHtML

class A: Base { override func f() {} }
来源：http://www.m.share.hesvh.cn/Article/details/gmbfrqutd.sHtML

[T27] Swift：错误处理
来源：http://m.share.hesvh.cn/Article/details/geubczrjz.sHtML

do { try f() } catch { print(error) }
来源：http://www.m.share.fehbvm.com/Article/details/gurgznqyh.sHtML

[T28] Swift：枚举
来源：http://www.share.fehbvm.com/Article/details/gbahmnrzo.sHtML

enum Color { case red, green }
来源：http://www.share.hesvh.cn/Article/details/gajcqsxpv.sHtML

[T29] Swift：guard 提前返回
来源：http://www.share.fehbvm.com/Article/details/gjohduija.sHtML

guard let x = opt else { return }
来源：http://3g.zdbjq.cn/Article/details/gsqlbrxll.sHtML

[T30] Swift：协议
来源：http://m.share.hesvh.cn/Article/details/gutivpyvc.sHtML

protocol Shape { func area() -> Double }
来源：http://mobile.zdbjq.cn/Article/details/gmujnagpq.sHtML

[T31] Lua：Hello World
来源：http://wap.fehbvm.com/Article/details/gbhinkcxv.sHtML

print("Hello")
来源：http://baike.hesvh.cn/Article/details/gsivrfgdx.sHtML

[T32] Lua：局部变量
来源：http://www.share.fehbvm.com/Article/details/gtyujuiww.sHtML

local a = 1
来源：http://www.blog.fehbvm.com/Article/details/ggkkrdrou.sHtML

[T33] Lua：表（数组）
来源：http://3g.hesvh.cn/Article/details/gtlequluf.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://m.share.zdbjq.cn/Article/details/gavuqqngz.sHtML

[T34] Lua：遍历表
来源：http://m.share.fehbvm.com/Article/details/gbrpfuuuv.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.fehbvm.com/Article/details/gqzehiajb.sHtML

[T35] Lua：字典表
来源：http://read.share.zdbjq.cn/Article/details/ghmooiehf.sHtML

local d = { a = 1 };  d.b = 2
来源：http://mobile.fehbvm.com/Article/details/geuvrchlf.sHtML

[T36] Lua：函数
来源：http://3g.fehbvm.com/Article/details/ghqbbgwki.sHtML

function add(a, b) return a + b end
来源：http://blog.zdbjq.cn/Article/details/gggrcczxh.sHtML

[T37] Lua：字符串拼接
来源：http://wap.hesvh.cn/Article/details/gxkpinkve.sHtML

"a" .. "b"
来源：http://m.share.fehbvm.com/Article/details/gcouyctid.sHtML

[T38] Lua：条件
来源：http://m.share.hesvh.cn/Article/details/gtcrpcktp.sHtML

if x > 0 then print("正") end
来源：http://www.share.fehbvm.com/Article/details/gkncundnq.sHtML


<!-- 参考信息 -->