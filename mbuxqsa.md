代发 wailian999

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.fanxiaobao.xyz/Article/details/gricvprcp.sHtML

[R34] 退出时清理
来源：http://blog.fanxiaobao.xyz/Article/details/gohfxjein.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.fanxiaobao.xyz/Article/details/goncwzmww.sHtML

[R35] 后台执行并等待
来源：http://www.share.fanxiaobao.xyz/Article/details/gwqsvjnet.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.fanxiaobao.xyz/Article/details/gpeavlzan.sHtML

[R36] 并发执行多个任务
来源：http://blog.fanxiaobao.xyz/Article/details/giukfvpec.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.fanxiaobao.xyz/Article/details/gnqdwmldj.sHtML

[R37] 把输出赋给变量
来源：http://baike.fanxiaobao.xyz/Article/details/gihdkbbug.sHtML

files=$(ls -1)
来源：http://wap.fanxiaobao.xyz/Article/details/gvxalpwvj.sHtML

[R38] 管道串联
来源：http://wap.fanxiaobao.xyz/Article/details/gstqosmpu.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.fanxiaobao.xyz/Article/details/gsynmejbs.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.fanxiaobao.xyz/Article/details/gdmhmkfnh.sHtML

cmd > out.log 2>&1
来源：http://wap.fanxiaobao.xyz/Article/details/gfvzglqhb.sHtML

[R40] 追加写日志
来源：http://mobile.fanxiaobao.xyz/Article/details/gfpoaajqq.sHtML

echo "log" >> out.log
来源：http://3g.fanxiaobao.xyz/Article/details/gvbzuxchd.sHtML

[R41] 丢弃输出
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnroytspz.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.fanxiaobao.xyz/Article/details/ghjbessbz.sHtML

[R42] 输入重定向
来源：http://wap.fanxiaobao.xyz/Article/details/gqdfpqyyw.sHtML

wc -l < a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkszfkihp.sHtML

[R43] 按名字查找文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gkthyifru.sHtML

find . -name "*.log" -type f
来源：http://3g.fanxiaobao.xyz/Article/details/gontnspwq.sHtML

[R44] 按修改时间查找
来源：http://www.share.fanxiaobao.xyz/Article/details/gsbroutlw.sHtML

find . -mtime -7 -type f
来源：http://3g.fanxiaobao.xyz/Article/details/giqgqbpmz.sHtML

[R45] 批量删除
来源：http://www.share.fanxiaobao.xyz/Article/details/gdsgiesbz.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmvihrnfc.sHtML

[R46] 递归替换文件内容
来源：http://read.share.fanxiaobao.xyz/Article/details/gkgacgeqa.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.fanxiaobao.xyz/Article/details/gzocugmul.sHtML

[R47] sed 单行替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gsfhwqgdc.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/glwfblfzw.sHtML

[R48] awk 取指定列
来源：http://3g.fanxiaobao.xyz/Article/details/glpweesen.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gqiuiewxh.sHtML

[R49] awk 带条件
来源：http://m.share.fanxiaobao.xyz/Article/details/gksedsfsh.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.fanxiaobao.xyz/Article/details/gpyfpiwla.sHtML

[R50] awk 求和
来源：http://baike.fanxiaobao.xyz/Article/details/gustdakkd.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/glswbwxfp.sHtML

[R51] 排序去重取前几
来源：http://m.share.fanxiaobao.xyz/Article/details/guwbyxgmp.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.fanxiaobao.xyz/Article/details/goobkslgp.sHtML

[R52] 统计行数
来源：http://read.share.fanxiaobao.xyz/Article/details/gtxwhbipd.sHtML

wc -l a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gyafsnfna.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.fanxiaobao.xyz/Article/details/gduppcvxa.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.fanxiaobao.xyz/Article/details/gjhxllgvq.sHtML

[R54] 比较两个文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gqxdejedz.sHtML

diff a.txt b.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gzcxdjqnc.sHtML

[R55] 压缩与解压
来源：http://mobile.fanxiaobao.xyz/Article/details/gxmppmfek.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.fanxiaobao.xyz/Article/details/gjbwujbqc.sHtML

[R56] 远程拷贝
来源：http://3g.fanxiaobao.xyz/Article/details/gpbodmgsc.sHtML

scp file user@host:/path/
来源：http://m.share.fanxiaobao.xyz/Article/details/gfxjhpuxt.sHtML

[R57] 远程执行命令
来源：http://www.share.fanxiaobao.xyz/Article/details/giyfqicuw.sHtML

ssh user@host 'uptime'
来源：http://read.share.fanxiaobao.xyz/Article/details/gtcuapcwc.sHtML

[R58] 下载文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gqzknrjlr.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.fanxiaobao.xyz/Article/details/gluoevwkl.sHtML

[R59] 发 POST JSON
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdduefkqh.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.fanxiaobao.xyz/Article/details/guuslxiwo.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaibpwoav.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.fanxiaobao.xyz/Article/details/glhwdggtk.sHtML

[R61] 磁盘占用
来源：http://blog.fanxiaobao.xyz/Article/details/ghcseoqsc.sHtML

df -h;  du -sh *
来源：http://mobile.fanxiaobao.xyz/Article/details/gsyqtikqh.sHtML

[R62] 找最占空间的文件
来源：http://m.share.fanxiaobao.xyz/Article/details/ghznvevku.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.fanxiaobao.xyz/Article/details/gwpkxdqmo.sHtML

[R63] 内存与进程
来源：http://3g.fanxiaobao.xyz/Article/details/gleyfoxjv.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.fanxiaobao.xyz/Article/details/gbxkkgeii.sHtML

[R64] 结束进程
来源：http://3g.fanxiaobao.xyz/Article/details/gvzmmehfi.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.fanxiaobao.xyz/Article/details/gyzehrcse.sHtML

[R65] 查看端口占用
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghouvunzf.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.fanxiaobao.xyz/Article/details/gigqqpbce.sHtML

[R66] 定时任务
来源：http://blog.fanxiaobao.xyz/Article/details/grenrldrh.sHtML

crontab -e;  crontab -l
来源：http://blog.fanxiaobao.xyz/Article/details/gjyizwciu.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvmcevasn.sHtML

openssl rand -hex 16
来源：http://www.blog.fanxiaobao.xyz/Article/details/gefakurfg.sHtML

[R68] 计算文件校验值
来源：http://blog.fanxiaobao.xyz/Article/details/gsjgeuilm.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gdkfhptrk.sHtML

[R69] 生成随机密码
来源：http://baike.fanxiaobao.xyz/Article/details/gijfhkdzf.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpzqrbely.sHtML

[R70] 时间戳与互转
来源：http://wap.fanxiaobao.xyz/Article/details/gzqdekgpu.sHtML

date +%s;  date -d @1700000000
来源：http://3g.fanxiaobao.xyz/Article/details/greoeqjio.sHtML

[R71] 日期格式化
来源：http://baike.fanxiaobao.xyz/Article/details/gusbrvxpp.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.fanxiaobao.xyz/Article/details/gjupkyfji.sHtML

[R72] 等待端口就绪
来源：http://read.share.fanxiaobao.xyz/Article/details/gomiglhtj.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdroncrau.sHtML

[R73] 分割大日志
来源：http://read.share.fanxiaobao.xyz/Article/details/gwyafvwkr.sHtML

split -l 1000 big.log part_
来源：http://www.blog.fanxiaobao.xyz/Article/details/gafzwseti.sHtML

[R74] 批量重命名
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggfgjykrh.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaaybvtqd.sHtML

[R75] 导出环境变量
来源：http://baike.fanxiaobao.xyz/Article/details/gpmedymns.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.fanxiaobao.xyz/Article/details/gnduqusop.sHtML

[R76] 使用临时文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/guofispdn.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fanxiaobao.xyz/Article/details/gbqjpltqw.sHtML

[R77] 读取用户输入
来源：http://3g.fanxiaobao.xyz/Article/details/gdvwqrxzy.sHtML

read -rp "请输入: " ans
来源：http://www.share.fanxiaobao.xyz/Article/details/gtbkzeqtb.sHtML

[R78] 交互式菜单
来源：http://m.share.fanxiaobao.xyz/Article/details/gpbbkzfxa.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.fanxiaobao.xyz/Article/details/gruxfresi.sHtML

[R79] 解析命令行选项
来源：http://wap.fanxiaobao.xyz/Article/details/gatbbnufn.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnryhfpcs.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwcxlynbm.sHtML

time ./run.sh
来源：http://m.share.fanxiaobao.xyz/Article/details/gmoiafqvh.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gelavgahi.sHtML

S. C / C++ 专题
来源：http://mobile.fanxiaobao.xyz/Article/details/gpsgtqqin.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gbehdbzzs.sHtML

[S01] C：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzgcvblmh.sHtML

#include <stdio.h>
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwvgrlels.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gduemwcal.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.fanxiaobao.xyz/Article/details/gfgrciwpw.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.fanxiaobao.xyz/Article/details/ghjnkylwd.sHtML

[S03] C：读入整数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbswanmjy.sHtML

int x; scanf("%d", &x);
来源：http://m.share.fanxiaobao.xyz/Article/details/gjogcajun.sHtML

[S04] C：字符串复制
来源：http://www.share.fanxiaobao.xyz/Article/details/ggywxfnch.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.fanxiaobao.xyz/Article/details/gemiwqzju.sHtML

[S05] C：字符串长度
来源：http://www.share.fanxiaobao.xyz/Article/details/goeqjlngo.sHtML

strlen(s)
来源：http://3g.fanxiaobao.xyz/Article/details/gmjhlbdzo.sHtML

[S06] C：字符串比较
来源：http://read.share.fanxiaobao.xyz/Article/details/ggwtcsqoz.sHtML

strcmp(a, b) == 0
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghwwrefkb.sHtML

[S07] C：数组遍历求和
来源：http://www.share.fanxiaobao.xyz/Article/details/gcorltmju.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gszzvbqai.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.fanxiaobao.xyz/Article/details/gktzbltgc.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.fanxiaobao.xyz/Article/details/gtqexcjsc.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.fanxiaobao.xyz/Article/details/gwtolmiru.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.fanxiaobao.xyz/Article/details/gmezlywhi.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gefhqhodv.sHtML

int *p = &a;  *p = 5;
来源：http://3g.fanxiaobao.xyz/Article/details/gqyrrgovl.sHtML

[S11] C：逐行读文件
来源：http://blog.fanxiaobao.xyz/Article/details/gyvxrrlih.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.fanxiaobao.xyz/Article/details/ggdtfhccx.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.fanxiaobao.xyz/Article/details/gezyccopb.sHtML

fclose(f);
来源：http://3g.fanxiaobao.xyz/Article/details/giuwaoccl.sHtML

[S12] C：写文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gwlyhvpbc.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.fanxiaobao.xyz/Article/details/gtpwqcbql.sHtML

[S13] C：宏定义
来源：http://www.share.fanxiaobao.xyz/Article/details/gviikykpf.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzbtslszj.sHtML

[S14] C：枚举
来源：http://www.share.fanxiaobao.xyz/Article/details/giuawfwpn.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcdehrfln.sHtML

[S15] C：类型转换
来源：http://www.share.fanxiaobao.xyz/Article/details/gnbcxhsre.sHtML

(double) a / b
来源：http://mobile.fanxiaobao.xyz/Article/details/gzcysrwpe.sHtML

[S16] C：位操作置位
来源：http://read.share.fanxiaobao.xyz/Article/details/grdzpwoch.sHtML

x |= (1 << 3);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guokhrsnv.sHtML

[S17] C：安全拼接字符串
来源：http://wap.fanxiaobao.xyz/Article/details/ggkszxgif.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.fanxiaobao.xyz/Article/details/gdiyuqevl.sHtML

[S18] C：命令行参数
来源：http://baike.fanxiaobao.xyz/Article/details/gntgfygci.sHtML

int main(int argc, char **argv)
来源：http://read.share.fanxiaobao.xyz/Article/details/gvphvtbgs.sHtML

[S19] C：快速排序
来源：http://wap.fanxiaobao.xyz/Article/details/gjzneerrq.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.fanxiaobao.xyz/Article/details/gctwxxuma.sHtML

[S20] C：二分查找
来源：http://read.share.fanxiaobao.xyz/Article/details/gjsbhbapd.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.fanxiaobao.xyz/Article/details/gtnsqvaqg.sHtML

[S21] C：字符类别判断
来源：http://read.share.fanxiaobao.xyz/Article/details/gafegpdzj.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdtfitjfz.sHtML

[S22] C：字符串转数字
来源：http://blog.fanxiaobao.xyz/Article/details/gofxmkpqy.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.fanxiaobao.xyz/Article/details/gstsryyvv.sHtML

[S23] C：随机数
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghchnirnl.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.fanxiaobao.xyz/Article/details/guoxtmuzz.sHtML

[S24] C：获取本地时间
来源：http://www.share.fanxiaobao.xyz/Article/details/giqsqyoqc.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpzrfwlut.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gburucfel.sHtML

memcpy(dst, src, n);
来源：http://baike.fanxiaobao.xyz/Article/details/gigsrmyfd.sHtML

[S26] C：内存清零
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpbwgpxjt.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggxzrucgx.sHtML

[S27] C：定义常量
来源：http://wap.fanxiaobao.xyz/Article/details/gvwjlobuo.sHtML

const double PI = 3.14159;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsglotqzz.sHtML

[S28] C：静态变量
来源：http://m.share.fanxiaobao.xyz/Article/details/geaxbolth.sHtML

static int counter = 0;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdjvrfanb.sHtML

[S29] C：变参函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gtwsucrpw.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.fanxiaobao.xyz/Article/details/goxspxzte.sHtML

[S30] C：头文件保护
来源：http://read.share.fanxiaobao.xyz/Article/details/groluzorj.sHtML

#ifndef X_H
来源：http://mobile.fanxiaobao.xyz/Article/details/gizycbxaz.sHtML

#define X_H
来源：http://www.share.fanxiaobao.xyz/Article/details/gxdzygaiq.sHtML

#endif
来源：http://blog.fanxiaobao.xyz/Article/details/gipcskprz.sHtML

[S31] C++：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/glfiwqvep.sHtML

#include <iostream>
来源：http://www.share.fanxiaobao.xyz/Article/details/gmiwbtvev.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gqwreveff.sHtML

[S32] C++：字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcnnjhlre.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.fanxiaobao.xyz/Article/details/gmmdvfymq.sHtML

[S33] C++：vector 增删
来源：http://read.share.fanxiaobao.xyz/Article/details/guyconztt.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqeigjuqt.sHtML

[S34] C++：遍历 vector
来源：http://3g.fanxiaobao.xyz/Article/details/gyityukhc.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gmvbzuizi.sHtML

[S35] C++：map
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcxaylsnc.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gbpknkcix.sHtML

[S36] C++：unordered_map
来源：http://blog.fanxiaobao.xyz/Article/details/gpntyutgz.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.fanxiaobao.xyz/Article/details/goenbrjeb.sHtML

[S37] C++：set
来源：http://www.blog.fanxiaobao.xyz/Article/details/goffdlrjf.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcwhchihq.sHtML

[S38] C++：排序
来源：http://baike.fanxiaobao.xyz/Article/details/gsjlhuthe.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.fanxiaobao.xyz/Article/details/gqqcoosfc.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpmwqkkzw.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gofakgdvq.sHtML

[S40] C++：查找元素
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsehwvzoi.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsdvmfrdo.sHtML

[S41] C++：类与构造函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gurwigtzf.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtsqcqaft.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gsdhvsnoo.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkyebfqmy.sHtML

[S43] C++：智能指针
来源：http://m.share.fanxiaobao.xyz/Article/details/gcnqhmxrv.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.fanxiaobao.xyz/Article/details/gztvkxckn.sHtML

[S44] C++：引用传参
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtkvqdyao.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gwjrglytq.sHtML

[S45] C++：lambda
来源：http://www.share.fanxiaobao.xyz/Article/details/guzzmqmxr.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.fanxiaobao.xyz/Article/details/gshfftskt.sHtML

[S46] C++：函数模板
来源：http://wap.fanxiaobao.xyz/Article/details/gfjqyangy.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.fanxiaobao.xyz/Article/details/gucfdysql.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.fanxiaobao.xyz/Article/details/gwqeghiwc.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gczovtfeo.sHtML

[S48] C++：逐行读文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gbrruazsz.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.fanxiaobao.xyz/Article/details/gulvcqvdk.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.fanxiaobao.xyz/Article/details/gaelrridr.sHtML

[S49] C++：写文件
来源：http://baike.fanxiaobao.xyz/Article/details/gxzoyxkxw.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.fanxiaobao.xyz/Article/details/gkudxeqhg.sHtML

[S50] C++：格式化数字
来源：http://3g.fanxiaobao.xyz/Article/details/gvyinfwbw.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.fanxiaobao.xyz/Article/details/gjhvitblb.sHtML

[S51] C++：显式类型转换
来源：http://wap.fanxiaobao.xyz/Article/details/gpewfrhus.sHtML

static_cast<double>(a) / b
来源：http://read.share.fanxiaobao.xyz/Article/details/ghsiqvall.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.fanxiaobao.xyz/Article/details/gtynsecvo.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnvwtotou.sHtML

[S53] C++：移动语义
来源：http://baike.fanxiaobao.xyz/Article/details/gsomwcjpe.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.fanxiaobao.xyz/Article/details/gdgkbvpru.sHtML

[S54] C++：异常处理
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtdlkaasb.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjaialgas.sHtML

[S55] C++：结构化绑定
来源：http://read.share.fanxiaobao.xyz/Article/details/ghempvfjs.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.fanxiaobao.xyz/Article/details/gkkscohst.sHtML

[S56] C++：optional
来源：http://blog.fanxiaobao.xyz/Article/details/gpdbyoazt.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.fanxiaobao.xyz/Article/details/gnfgiyepl.sHtML

[S57] C++：编译期常量
来源：http://wap.fanxiaobao.xyz/Article/details/gpsxevynx.sHtML

constexpr int N = 10;
来源：http://blog.fanxiaobao.xyz/Article/details/gyitmzzlg.sHtML

[S58] C++：命名空间
来源：http://3g.fanxiaobao.xyz/Article/details/gpijrhvdn.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.fanxiaobao.xyz/Article/details/gaapnqqsp.sHtML

[S59] C++：静态断言
来源：http://www.share.fanxiaobao.xyz/Article/details/gqssuhnwc.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.fanxiaobao.xyz/Article/details/gknvtozts.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.fanxiaobao.xyz/Article/details/gbxikbyzz.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.fanxiaobao.xyz/Article/details/guowflmos.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvmimjajv.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.fanxiaobao.xyz/Article/details/gpqzzqieq.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gerpfonej.sHtML

[T01] Kotlin：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gvfxafkih.sHtML

println("Hello")
来源：http://m.share.fanxiaobao.xyz/Article/details/gqlbxwdxq.sHtML

[T02] Kotlin：变量
来源：http://blog.fanxiaobao.xyz/Article/details/ghlynzlqw.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.fanxiaobao.xyz/Article/details/gutjmpayf.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.fanxiaobao.xyz/Article/details/ghtfrqxsw.sHtML

"值: $b"
来源：http://blog.fanxiaobao.xyz/Article/details/gxlduhows.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbsqscaby.sHtML

val n: String? = null;  n?.length
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gldvpbdxu.sHtML

[T05] Kotlin：when 表达式
来源：http://wap.fanxiaobao.xyz/Article/details/grienyxom.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.fanxiaobao.xyz/Article/details/gnexdbynj.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.fanxiaobao.xyz/Article/details/gejtuniil.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.fanxiaobao.xyz/Article/details/gahanaucl.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.fanxiaobao.xyz/Article/details/gukuqxxnm.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gciiqplzt.sHtML

[T08] Kotlin：数据类
来源：http://baike.fanxiaobao.xyz/Article/details/grdqlplug.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.fanxiaobao.xyz/Article/details/gcgcarbcm.sHtML

[T09] Kotlin：扩展函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gumcqrmwp.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.fanxiaobao.xyz/Article/details/gokpqsqzn.sHtML

[T10] Kotlin：默认参数
来源：http://blog.fanxiaobao.xyz/Article/details/gcltfwwie.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.fanxiaobao.xyz/Article/details/gvcdnzaug.sHtML

[T11] Kotlin：协程
来源：http://wap.fanxiaobao.xyz/Article/details/gysuypgya.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.fanxiaobao.xyz/Article/details/gofxjmbfc.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjglmqher.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.fanxiaobao.xyz/Article/details/groldqzkz.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.fanxiaobao.xyz/Article/details/godhhlffj.sHtML

val m = mapOf("a" to 1)
来源：http://www.share.fanxiaobao.xyz/Article/details/gosvsqcbg.sHtML

[T14] Kotlin：循环
来源：http://3g.fanxiaobao.xyz/Article/details/gghgbvjbf.sHtML

for (i in 1..10) println(i)
来源：http://www.share.fanxiaobao.xyz/Article/details/gxskauloh.sHtML

[T15] Kotlin：接口
来源：http://read.share.fanxiaobao.xyz/Article/details/gpgupxdac.sHtML

interface Shape { fun area(): Double }
来源：http://m.share.fanxiaobao.xyz/Article/details/ggokyeavh.sHtML

[T16] Swift：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geznwkqmc.sHtML

print("Hello")
来源：http://wap.fanxiaobao.xyz/Article/details/gcpkhbvyu.sHtML

[T17] Swift：变量与常量
来源：http://baike.fanxiaobao.xyz/Article/details/gzsugxbxn.sHtML

var a = 1;  let b = 2
来源：http://www.share.fanxiaobao.xyz/Article/details/gfvyjozgb.sHtML

[T18] Swift：字符串插值
来源：http://www.share.fanxiaobao.xyz/Article/details/glqoxmrsm.sHtML

"值: \(b)"
来源：http://blog.fanxiaobao.xyz/Article/details/guyjcixpr.sHtML

[T19] Swift：可选绑定
来源：http://read.share.fanxiaobao.xyz/Article/details/gubonqogi.sHtML

if let n = opt { print(n) }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkgunnpjr.sHtML

[T20] Swift：数组操作
来源：http://blog.fanxiaobao.xyz/Article/details/gvzgpusbg.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://mobile.fanxiaobao.xyz/Article/details/gdpqfwqtc.sHtML

[T21] Swift：遍历
来源：http://3g.fanxiaobao.xyz/Article/details/gbgoxplfn.sHtML

for x in a { print(x) }
来源：http://m.share.fanxiaobao.xyz/Article/details/gdixkbzqz.sHtML

[T22] Swift：字典
来源：http://wap.fanxiaobao.xyz/Article/details/ghzzjqsza.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://m.share.fanxiaobao.xyz/Article/details/gazimoiss.sHtML

[T23] Swift：函数
来源：http://baike.fanxiaobao.xyz/Article/details/gtylzpqib.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gowbidszp.sHtML

[T24] Swift：闭包
来源：http://3g.fanxiaobao.xyz/Article/details/gqdwvtjwm.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.fanxiaobao.xyz/Article/details/gfyrnqqcb.sHtML

[T25] Swift：结构体
来源：http://m.share.fanxiaobao.xyz/Article/details/gtngpuiag.sHtML

struct P { var x: Int }
来源：http://baike.fanxiaobao.xyz/Article/details/grjtifmta.sHtML

[T26] Swift：类与重写
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvqlhklnl.sHtML

class A: Base { override func f() {} }
来源：http://wap.fanxiaobao.xyz/Article/details/gijzmebfk.sHtML

[T27] Swift：错误处理
来源：http://baike.fanxiaobao.xyz/Article/details/gksgfmkly.sHtML

do { try f() } catch { print(error) }
来源：http://baike.fanxiaobao.xyz/Article/details/gqfgnkjjc.sHtML

[T28] Swift：枚举
来源：http://www.share.fanxiaobao.xyz/Article/details/gbxjnefsd.sHtML

enum Color { case red, green }
来源：http://www.share.fanxiaobao.xyz/Article/details/grvvlbosh.sHtML

[T29] Swift：guard 提前返回
来源：http://www.blog.fanxiaobao.xyz/Article/details/giecvjttn.sHtML

guard let x = opt else { return }
来源：http://read.share.fanxiaobao.xyz/Article/details/gualqxtty.sHtML

[T30] Swift：协议
来源：http://baike.fanxiaobao.xyz/Article/details/ggomvoadk.sHtML

protocol Shape { func area() -> Double }
来源：http://baike.fanxiaobao.xyz/Article/details/gfbsahdim.sHtML

[T31] Lua：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gjgncgroj.sHtML

print("Hello")
来源：http://m.share.fanxiaobao.xyz/Article/details/gqzoadpcb.sHtML

[T32] Lua：局部变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gjpnogkkx.sHtML

local a = 1
来源：http://wap.fanxiaobao.xyz/Article/details/gyxymlirf.sHtML

[T33] Lua：表（数组）
来源：http://read.share.fanxiaobao.xyz/Article/details/gfglomotg.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glcfbzddl.sHtML

[T34] Lua：遍历表
来源：http://blog.fanxiaobao.xyz/Article/details/gcsalpegf.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkrrtztrb.sHtML

[T35] Lua：字典表
来源：http://m.share.fanxiaobao.xyz/Article/details/gakbsojxu.sHtML

local d = { a = 1 };  d.b = 2
来源：http://blog.fanxiaobao.xyz/Article/details/gnlsawqdi.sHtML

[T36] Lua：函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpyvzeuxs.sHtML

function add(a, b) return a + b end
来源：http://read.share.fanxiaobao.xyz/Article/details/gnrbbxvex.sHtML


<!-- 参考信息 -->