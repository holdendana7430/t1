代发 wailian999

files=$(ls -1)
来源：http://baike.fanxiaobao.xyz/Article/details/grpniaonj.sHtML

[R38] 管道串联
来源：http://mobile.fanxiaobao.xyz/Article/details/gqjajtwfk.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.fanxiaobao.xyz/Article/details/ghvnkfkzn.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gogdatcid.sHtML

cmd > out.log 2>&1
来源：http://blog.fanxiaobao.xyz/Article/details/gucbfzmno.sHtML

[R40] 追加写日志
来源：http://blog.fanxiaobao.xyz/Article/details/gqqawwnlh.sHtML

echo "log" >> out.log
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggjlxmmsq.sHtML

[R41] 丢弃输出
来源：http://m.share.fanxiaobao.xyz/Article/details/geopxpnsl.sHtML

cmd >/dev/null 2>&1
来源：http://wap.fanxiaobao.xyz/Article/details/gglvxuvbe.sHtML

[R42] 输入重定向
来源：http://3g.fanxiaobao.xyz/Article/details/grmqcchwo.sHtML

wc -l < a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gcxzsimly.sHtML

[R43] 按名字查找文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gjgipisac.sHtML

find . -name "*.log" -type f
来源：http://mobile.fanxiaobao.xyz/Article/details/gpcyhlbbi.sHtML

[R44] 按修改时间查找
来源：http://baike.fanxiaobao.xyz/Article/details/gwlfvdiop.sHtML

find . -mtime -7 -type f
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggzocqogz.sHtML

[R45] 批量删除
来源：http://wap.fanxiaobao.xyz/Article/details/gvnkkykfy.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.fanxiaobao.xyz/Article/details/gayejmcxb.sHtML

[R46] 递归替换文件内容
来源：http://m.share.fanxiaobao.xyz/Article/details/gzeuryjnw.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.fanxiaobao.xyz/Article/details/gttthnuvo.sHtML

[R47] sed 单行替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaenevlty.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gklkcqyin.sHtML

[R48] awk 取指定列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcezdhtxz.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/groivmoam.sHtML

[R49] awk 带条件
来源：http://wap.fanxiaobao.xyz/Article/details/gjojuoudw.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.fanxiaobao.xyz/Article/details/glmslpxrb.sHtML

[R50] awk 求和
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnydnzpbg.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gaoayhtrs.sHtML

[R51] 排序去重取前几
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkjwstbhy.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.fanxiaobao.xyz/Article/details/gahobhxum.sHtML

[R52] 统计行数
来源：http://baike.fanxiaobao.xyz/Article/details/gztgwloni.sHtML

wc -l a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gcnvmxgcg.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.fanxiaobao.xyz/Article/details/gthctwwgk.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggturzdgu.sHtML

[R54] 比较两个文件
来源：http://blog.fanxiaobao.xyz/Article/details/gqenyrgus.sHtML

diff a.txt b.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gzxfcegnv.sHtML

[R55] 压缩与解压
来源：http://read.share.fanxiaobao.xyz/Article/details/gkgbntrdj.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.fanxiaobao.xyz/Article/details/gzgqkcozl.sHtML

[R56] 远程拷贝
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdlaycilh.sHtML

scp file user@host:/path/
来源：http://read.share.fanxiaobao.xyz/Article/details/gzeuqooil.sHtML

[R57] 远程执行命令
来源：http://blog.fanxiaobao.xyz/Article/details/gjxzwfagb.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwdkggnhs.sHtML

[R58] 下载文件
来源：http://m.share.fanxiaobao.xyz/Article/details/ghdgvfvpp.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.fanxiaobao.xyz/Article/details/gjzkdnnee.sHtML

[R59] 发 POST JSON
来源：http://www.share.fanxiaobao.xyz/Article/details/gzqsnelic.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.fanxiaobao.xyz/Article/details/gabsdlbwf.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.fanxiaobao.xyz/Article/details/gixwhqrzv.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.fanxiaobao.xyz/Article/details/gqfmduevs.sHtML

[R61] 磁盘占用
来源：http://m.share.fanxiaobao.xyz/Article/details/gskrkyhtw.sHtML

df -h;  du -sh *
来源：http://mobile.fanxiaobao.xyz/Article/details/gdskawqlf.sHtML

[R62] 找最占空间的文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gmzilvnzi.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.fanxiaobao.xyz/Article/details/gnnowcdan.sHtML

[R63] 内存与进程
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gckocerlg.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.fanxiaobao.xyz/Article/details/gnwejvgti.sHtML

[R64] 结束进程
来源：http://www.share.fanxiaobao.xyz/Article/details/gfhvfyris.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.fanxiaobao.xyz/Article/details/gdtkpmfte.sHtML

[R65] 查看端口占用
来源：http://3g.fanxiaobao.xyz/Article/details/gooukmxex.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.fanxiaobao.xyz/Article/details/ggqvyxhuo.sHtML

[R66] 定时任务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqsiilsez.sHtML

crontab -e;  crontab -l
来源：http://read.share.fanxiaobao.xyz/Article/details/guplpaknk.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.fanxiaobao.xyz/Article/details/ghwxfbxwc.sHtML

openssl rand -hex 16
来源：http://m.share.fanxiaobao.xyz/Article/details/gsifgduth.sHtML

[R68] 计算文件校验值
来源：http://m.share.fanxiaobao.xyz/Article/details/gmtmybnmu.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gpexqxumi.sHtML

[R69] 生成随机密码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvreflinj.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.fanxiaobao.xyz/Article/details/gxxbuvpox.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzpewizll.sHtML

date +%s;  date -d @1700000000
来源：http://baike.fanxiaobao.xyz/Article/details/gfeauzpbr.sHtML

[R71] 日期格式化
来源：http://3g.fanxiaobao.xyz/Article/details/giyazkisj.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.fanxiaobao.xyz/Article/details/gsmftxhtn.sHtML

[R72] 等待端口就绪
来源：http://www.share.fanxiaobao.xyz/Article/details/gwgogncbd.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gxclgseia.sHtML

[R73] 分割大日志
来源：http://blog.fanxiaobao.xyz/Article/details/gptsqzdhd.sHtML

split -l 1000 big.log part_
来源：http://m.share.fanxiaobao.xyz/Article/details/gyukmehyo.sHtML

[R74] 批量重命名
来源：http://baike.fanxiaobao.xyz/Article/details/gmlqtxxgk.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.fanxiaobao.xyz/Article/details/gynhrfjss.sHtML

[R75] 导出环境变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gepmdwcof.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.fanxiaobao.xyz/Article/details/ghsfgdepa.sHtML

[R76] 使用临时文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gzxklithl.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghdqiatlo.sHtML

[R77] 读取用户输入
来源：http://blog.fanxiaobao.xyz/Article/details/ggbajlrua.sHtML

read -rp "请输入: " ans
来源：http://read.share.fanxiaobao.xyz/Article/details/gjowipavm.sHtML

[R78] 交互式菜单
来源：http://baike.fanxiaobao.xyz/Article/details/gxchzqryh.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.fanxiaobao.xyz/Article/details/gjxudeitn.sHtML

[R79] 解析命令行选项
来源：http://blog.fanxiaobao.xyz/Article/details/ganmftxdk.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghijwzfjd.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.fanxiaobao.xyz/Article/details/gmbxaroxo.sHtML

time ./run.sh
来源：http://mobile.fanxiaobao.xyz/Article/details/gcpuurhct.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gnvpqrict.sHtML

S. C / C++ 专题
来源：http://blog.fanxiaobao.xyz/Article/details/gabwayyiy.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwjzwanua.sHtML

[S01] C：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gkyookmkr.sHtML

#include <stdio.h>
来源：http://www.share.fanxiaobao.xyz/Article/details/grilvdfeu.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.fanxiaobao.xyz/Article/details/gpkwviypt.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfxkduluy.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gipgmkylc.sHtML

[S03] C：读入整数
来源：http://read.share.fanxiaobao.xyz/Article/details/grsbyylnw.sHtML

int x; scanf("%d", &x);
来源：http://www.share.fanxiaobao.xyz/Article/details/gihejphhc.sHtML

[S04] C：字符串复制
来源：http://read.share.fanxiaobao.xyz/Article/details/gfsohlpbj.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.fanxiaobao.xyz/Article/details/gjuylnekq.sHtML

[S05] C：字符串长度
来源：http://www.share.fanxiaobao.xyz/Article/details/gqmwhhvsn.sHtML

strlen(s)
来源：http://www.share.fanxiaobao.xyz/Article/details/gtqanyekw.sHtML

[S06] C：字符串比较
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwjglioap.sHtML

strcmp(a, b) == 0
来源：http://blog.fanxiaobao.xyz/Article/details/grytxmbec.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gujqjmoln.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.fanxiaobao.xyz/Article/details/grhjabrru.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghdxritkg.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.fanxiaobao.xyz/Article/details/gcpgdwvyh.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.fanxiaobao.xyz/Article/details/gkxvspozq.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.fanxiaobao.xyz/Article/details/gbvckxdoz.sHtML

[S10] C：指针与解引用
来源：http://mobile.fanxiaobao.xyz/Article/details/gbkhjjuwu.sHtML

int *p = &a;  *p = 5;
来源：http://3g.fanxiaobao.xyz/Article/details/ghwfvwvdi.sHtML

[S11] C：逐行读文件
来源：http://baike.fanxiaobao.xyz/Article/details/gjtejednj.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.fanxiaobao.xyz/Article/details/gxvnstmei.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvunzyopq.sHtML

fclose(f);
来源：http://mobile.fanxiaobao.xyz/Article/details/gylyzzhyb.sHtML

[S12] C：写文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtlkmnqde.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.fanxiaobao.xyz/Article/details/gatgtyycs.sHtML

[S13] C：宏定义
来源：http://wap.fanxiaobao.xyz/Article/details/gjeynqfib.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.fanxiaobao.xyz/Article/details/gebahzwzd.sHtML

[S14] C：枚举
来源：http://blog.fanxiaobao.xyz/Article/details/glagllcrk.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.fanxiaobao.xyz/Article/details/gexcjtzmj.sHtML

[S15] C：类型转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggpvhpccr.sHtML

(double) a / b
来源：http://www.share.fanxiaobao.xyz/Article/details/gfdidagak.sHtML

[S16] C：位操作置位
来源：http://wap.fanxiaobao.xyz/Article/details/gzaazyuxl.sHtML

x |= (1 << 3);
来源：http://baike.fanxiaobao.xyz/Article/details/gzmxttaiw.sHtML

[S17] C：安全拼接字符串
来源：http://blog.fanxiaobao.xyz/Article/details/gvjmqcwae.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glbhvqsug.sHtML

[S18] C：命令行参数
来源：http://blog.fanxiaobao.xyz/Article/details/gyyzsygxs.sHtML

int main(int argc, char **argv)
来源：http://mobile.fanxiaobao.xyz/Article/details/ghznykzlv.sHtML

[S19] C：快速排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gusrbahjv.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.fanxiaobao.xyz/Article/details/gyzgpjcya.sHtML

[S20] C：二分查找
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gishakrif.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghkwvpdib.sHtML

[S21] C：字符类别判断
来源：http://blog.fanxiaobao.xyz/Article/details/gpfjhkybn.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.fanxiaobao.xyz/Article/details/gxdupfiar.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gujcnobbs.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.fanxiaobao.xyz/Article/details/gdsyeresp.sHtML

[S23] C：随机数
来源：http://m.share.fanxiaobao.xyz/Article/details/gzvepcnmi.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gourmiyie.sHtML

[S24] C：获取本地时间
来源：http://mobile.fanxiaobao.xyz/Article/details/gdyvxfckz.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gykllphgn.sHtML

[S25] C：内存拷贝
来源：http://www.share.fanxiaobao.xyz/Article/details/gnbycrpwx.sHtML

memcpy(dst, src, n);
来源：http://www.share.fanxiaobao.xyz/Article/details/gzcneaarq.sHtML

[S26] C：内存清零
来源：http://blog.fanxiaobao.xyz/Article/details/gcdryztej.sHtML

memset(a, 0, sizeof a);
来源：http://baike.fanxiaobao.xyz/Article/details/ggcnlkgkk.sHtML

[S27] C：定义常量
来源：http://read.share.fanxiaobao.xyz/Article/details/gdbchhnsx.sHtML

const double PI = 3.14159;
来源：http://3g.fanxiaobao.xyz/Article/details/gwkpgoamb.sHtML

[S28] C：静态变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gblabqkpp.sHtML

static int counter = 0;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goocetciu.sHtML

[S29] C：变参函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gbqoonwyz.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghuyezjqa.sHtML

[S30] C：头文件保护
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjshzrdep.sHtML

#ifndef X_H
来源：http://read.share.fanxiaobao.xyz/Article/details/gpstcoare.sHtML

#define X_H
来源：http://www.blog.fanxiaobao.xyz/Article/details/guwhittxg.sHtML

#endif
来源：http://baike.fanxiaobao.xyz/Article/details/gtixaaxbq.sHtML

[S31] C++：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gukilmaje.sHtML

#include <iostream>
来源：http://mobile.fanxiaobao.xyz/Article/details/ggqfuhpkd.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.fanxiaobao.xyz/Article/details/gnodnuslu.sHtML

[S32] C++：字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/gxyijqajm.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.fanxiaobao.xyz/Article/details/gnmkbzkqw.sHtML

[S33] C++：vector 增删
来源：http://3g.fanxiaobao.xyz/Article/details/gskobfvke.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtoccstyh.sHtML

[S34] C++：遍历 vector
来源：http://m.share.fanxiaobao.xyz/Article/details/gyrevakrg.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gktyyahfs.sHtML

[S35] C++：map
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjxuotzuh.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fanxiaobao.xyz/Article/details/gpdbrnadj.sHtML

[S36] C++：unordered_map
来源：http://wap.fanxiaobao.xyz/Article/details/gskbmodiw.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.fanxiaobao.xyz/Article/details/gzmetnshu.sHtML

[S37] C++：set
来源：http://wap.fanxiaobao.xyz/Article/details/grvmmjhqe.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxmnbuknh.sHtML

[S38] C++：排序
来源：http://3g.fanxiaobao.xyz/Article/details/gqfxezcwq.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.fanxiaobao.xyz/Article/details/gfufskzeh.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.fanxiaobao.xyz/Article/details/gdprmpqqk.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.fanxiaobao.xyz/Article/details/gnebwdjci.sHtML

[S40] C++：查找元素
来源：http://www.share.fanxiaobao.xyz/Article/details/gpretgfhl.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.fanxiaobao.xyz/Article/details/gcmcibubp.sHtML

[S41] C++：类与构造函数
来源：http://baike.fanxiaobao.xyz/Article/details/gqtywvxhk.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.fanxiaobao.xyz/Article/details/gfusgbkwp.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.fanxiaobao.xyz/Article/details/ggracoqxo.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.fanxiaobao.xyz/Article/details/gxocgrbnu.sHtML

[S43] C++：智能指针
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghbapelkj.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.fanxiaobao.xyz/Article/details/giheqgiaa.sHtML

[S44] C++：引用传参
来源：http://blog.fanxiaobao.xyz/Article/details/gywgcuiry.sHtML

void inc(int &x) { ++x; }
来源：http://baike.fanxiaobao.xyz/Article/details/getmpylly.sHtML

[S45] C++：lambda
来源：http://blog.fanxiaobao.xyz/Article/details/gvrqjpqho.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.fanxiaobao.xyz/Article/details/gmnolkocg.sHtML

[S46] C++：函数模板
来源：http://www.blog.fanxiaobao.xyz/Article/details/gimivblzv.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.fanxiaobao.xyz/Article/details/giqpmnitu.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghqousqcq.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gheqbywax.sHtML

[S48] C++：逐行读文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gwukmjoij.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gunlxzelq.sHtML

while (std::getline(in, line)) { }
来源：http://3g.fanxiaobao.xyz/Article/details/ganjbrcvw.sHtML

[S49] C++：写文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gcxenwlor.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.fanxiaobao.xyz/Article/details/gxjvhfaxn.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwhubtjdp.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.fanxiaobao.xyz/Article/details/gifrwrneq.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/grzxgetxw.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpwppeitm.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.fanxiaobao.xyz/Article/details/gjjnjsmib.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gylhqmgvx.sHtML

[S53] C++：移动语义
来源：http://www.share.fanxiaobao.xyz/Article/details/gyddhvvyg.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.fanxiaobao.xyz/Article/details/gqdktmolx.sHtML

[S54] C++：异常处理
来源：http://blog.fanxiaobao.xyz/Article/details/gfumskvap.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.fanxiaobao.xyz/Article/details/gdqmvbujr.sHtML

[S55] C++：结构化绑定
来源：http://blog.fanxiaobao.xyz/Article/details/gobrhfldb.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grgmmpbcv.sHtML

[S56] C++：optional
来源：http://blog.fanxiaobao.xyz/Article/details/gwvuiotlp.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.fanxiaobao.xyz/Article/details/gxlkapvcu.sHtML

[S57] C++：编译期常量
来源：http://blog.fanxiaobao.xyz/Article/details/glpetgkyu.sHtML

constexpr int N = 10;
来源：http://www.blog.fanxiaobao.xyz/Article/details/giwzkwrzf.sHtML

[S58] C++：命名空间
来源：http://blog.fanxiaobao.xyz/Article/details/gaooinwyt.sHtML

namespace ns { int f() { return 1; } }
来源：http://3g.fanxiaobao.xyz/Article/details/gptmklltr.sHtML

[S59] C++：静态断言
来源：http://baike.fanxiaobao.xyz/Article/details/ggzsekuwc.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.fanxiaobao.xyz/Article/details/gybsiohpk.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.fanxiaobao.xyz/Article/details/gcgobryrn.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.fanxiaobao.xyz/Article/details/gjqmocmbl.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gxnmxgpyv.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.fanxiaobao.xyz/Article/details/gvgnufvqy.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gekegdgxj.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gholpxjbn.sHtML

println("Hello")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxjtktpwv.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggwodmwpa.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.fanxiaobao.xyz/Article/details/gavwovuez.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.fanxiaobao.xyz/Article/details/gojpnyzti.sHtML

"值: $b"
来源：http://3g.fanxiaobao.xyz/Article/details/gmctqmyve.sHtML

[T04] Kotlin：空安全
来源：http://mobile.fanxiaobao.xyz/Article/details/ghibimaar.sHtML

val n: String? = null;  n?.length
来源：http://m.share.fanxiaobao.xyz/Article/details/gkdjnahhi.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.fanxiaobao.xyz/Article/details/grwmgnvrj.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.fanxiaobao.xyz/Article/details/gvvjklhgg.sHtML

[T06] Kotlin：集合映射
来源：http://3g.fanxiaobao.xyz/Article/details/gmikuxngf.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.fanxiaobao.xyz/Article/details/gnchxtozy.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.fanxiaobao.xyz/Article/details/govsrqljz.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.fanxiaobao.xyz/Article/details/gyfqdpsri.sHtML

[T08] Kotlin：数据类
来源：http://wap.fanxiaobao.xyz/Article/details/gsgrcjfgp.sHtML

data class User(val name: String, val age: Int)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpgyaiftq.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtcexkzha.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.fanxiaobao.xyz/Article/details/gojtnzquj.sHtML

[T10] Kotlin：默认参数
来源：http://baike.fanxiaobao.xyz/Article/details/gqcahwhrb.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.fanxiaobao.xyz/Article/details/gqxlzvflz.sHtML

[T11] Kotlin：协程
来源：http://m.share.fanxiaobao.xyz/Article/details/gazkyinas.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.share.fanxiaobao.xyz/Article/details/gxcjnssuc.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghfrnmwfc.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.fanxiaobao.xyz/Article/details/gzwtdjaan.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.fanxiaobao.xyz/Article/details/gxrucmjvr.sHtML

val m = mapOf("a" to 1)
来源：http://www.share.fanxiaobao.xyz/Article/details/gnterzamw.sHtML

[T14] Kotlin：循环
来源：http://read.share.fanxiaobao.xyz/Article/details/gmqynsqxz.sHtML

for (i in 1..10) println(i)
来源：http://3g.fanxiaobao.xyz/Article/details/gbwyaoeuu.sHtML

[T15] Kotlin：接口
来源：http://mobile.fanxiaobao.xyz/Article/details/gdsngbxpk.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjmcwmwke.sHtML

[T16] Swift：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxuoxtcqk.sHtML

print("Hello")
来源：http://wap.fanxiaobao.xyz/Article/details/gdrfmekns.sHtML

[T17] Swift：变量与常量
来源：http://mobile.fanxiaobao.xyz/Article/details/gsbqmnkvv.sHtML

var a = 1;  let b = 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghvqwyxlc.sHtML

[T18] Swift：字符串插值
来源：http://www.share.fanxiaobao.xyz/Article/details/gwfnebcaz.sHtML

"值: \(b)"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzoxizdit.sHtML

[T19] Swift：可选绑定
来源：http://3g.fanxiaobao.xyz/Article/details/glcqrhhwk.sHtML

if let n = opt { print(n) }
来源：http://read.share.fanxiaobao.xyz/Article/details/ghmvndxvp.sHtML

[T20] Swift：数组操作
来源：http://mobile.fanxiaobao.xyz/Article/details/gmxdohgdj.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://baike.fanxiaobao.xyz/Article/details/guzitusjs.sHtML

[T21] Swift：遍历
来源：http://blog.fanxiaobao.xyz/Article/details/gyyzdivmv.sHtML

for x in a { print(x) }
来源：http://3g.fanxiaobao.xyz/Article/details/gienznwme.sHtML

[T22] Swift：字典
来源：http://mobile.fanxiaobao.xyz/Article/details/gzivyizpv.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://read.share.fanxiaobao.xyz/Article/details/gpavfofwu.sHtML

[T23] Swift：函数
来源：http://3g.fanxiaobao.xyz/Article/details/gprzamwal.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.fanxiaobao.xyz/Article/details/glqjrbbhd.sHtML

[T24] Swift：闭包
来源：http://m.share.fanxiaobao.xyz/Article/details/gifklojla.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.share.fanxiaobao.xyz/Article/details/graatpxcm.sHtML

[T25] Swift：结构体
来源：http://mobile.fanxiaobao.xyz/Article/details/gjsbqwaeg.sHtML

struct P { var x: Int }
来源：http://read.share.fanxiaobao.xyz/Article/details/gxxlapbfr.sHtML

[T26] Swift：类与重写
来源：http://wap.fanxiaobao.xyz/Article/details/gncaltatn.sHtML

class A: Base { override func f() {} }
来源：http://read.share.fanxiaobao.xyz/Article/details/gyddbqbqq.sHtML

[T27] Swift：错误处理
来源：http://mobile.fanxiaobao.xyz/Article/details/ggxhpqzvc.sHtML

do { try f() } catch { print(error) }
来源：http://wap.fanxiaobao.xyz/Article/details/gzyozyajo.sHtML

[T28] Swift：枚举
来源：http://mobile.fanxiaobao.xyz/Article/details/gdtnctpns.sHtML

enum Color { case red, green }
来源：http://baike.fanxiaobao.xyz/Article/details/gfibflfid.sHtML

[T29] Swift：guard 提前返回
来源：http://www.blog.fanxiaobao.xyz/Article/details/gilezlcsu.sHtML

guard let x = opt else { return }
来源：http://read.share.fanxiaobao.xyz/Article/details/gmeunhzlo.sHtML

[T30] Swift：协议
来源：http://wap.fanxiaobao.xyz/Article/details/gsuyeejmx.sHtML

protocol Shape { func area() -> Double }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcshdkgau.sHtML

[T31] Lua：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gpeueahqe.sHtML

print("Hello")
来源：http://wap.fanxiaobao.xyz/Article/details/gyhhlcdlb.sHtML

[T32] Lua：局部变量
来源：http://blog.fanxiaobao.xyz/Article/details/gnxqhwjvz.sHtML

local a = 1
来源：http://www.share.fanxiaobao.xyz/Article/details/giwydbbva.sHtML

[T33] Lua：表（数组）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtdflwsoi.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://3g.fanxiaobao.xyz/Article/details/gtmtsphlu.sHtML

[T34] Lua：遍历表
来源：http://mobile.fanxiaobao.xyz/Article/details/gbkopqvnw.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://3g.fanxiaobao.xyz/Article/details/glrlqsqzv.sHtML

[T35] Lua：字典表
来源：http://wap.fanxiaobao.xyz/Article/details/gtlxpybut.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzfolnsai.sHtML

[T36] Lua：函数
来源：http://blog.fanxiaobao.xyz/Article/details/ggqmxiuwt.sHtML

function add(a, b) return a + b end
来源：http://www.blog.fanxiaobao.xyz/Article/details/geypfwbvt.sHtML

[T37] Lua：字符串拼接
来源：http://wap.fanxiaobao.xyz/Article/details/grbnifjvg.sHtML

"a" .. "b"
来源：http://mobile.fanxiaobao.xyz/Article/details/gjpihhhjk.sHtML

[T38] Lua：条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzqkqlxin.sHtML

if x > 0 then print("正") end
来源：http://wap.fanxiaobao.xyz/Article/details/gpydokway.sHtML

[T39] Lua：模式匹配
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxqykhudz.sHtML

string.find(s, "%d+")
来源：http://read.share.fanxiaobao.xyz/Article/details/gspjxrmvq.sHtML

[T40] Lua：元表
来源：http://3g.fanxiaobao.xyz/Article/details/gmhiajirs.sHtML

setmetatable({}, { __index = base })
来源：http://mobile.fanxiaobao.xyz/Article/details/gmicpguev.sHtML


<!-- 参考信息 -->