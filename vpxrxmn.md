代发 wailian999

f() { local x=1; echo "$x"; }
来源：http://wap.fehbvm.com/Article/details/gfhohzcyo.sHtML

[R32] 参数个数校验
来源：http://www.m.share.fehbvm.com/Article/details/gnhdpdwmj.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.hesvh.cn/Article/details/glsozibrs.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.fehbvm.com/Article/details/gajiwwbad.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.zdbjq.cn/Article/details/gjiaasiaz.sHtML

[R34] 退出时清理
来源：http://www.blog.zdbjq.cn/Article/details/gyxoonvrw.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fehbvm.com/Article/details/gedyotnku.sHtML

[R35] 后台执行并等待
来源：http://3g.zdbjq.cn/Article/details/gfliyijmm.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.hesvh.cn/Article/details/ghxnoiozp.sHtML

[R36] 并发执行多个任务
来源：http://3g.zdbjq.cn/Article/details/gdqwamtao.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.fehbvm.com/Article/details/gbbeequea.sHtML

[R37] 把输出赋给变量
来源：http://www.share.fehbvm.com/Article/details/ghkefiiji.sHtML

files=$(ls -1)
来源：http://3g.fehbvm.com/Article/details/gkixoxwnm.sHtML

[R38] 管道串联
来源：http://3g.hesvh.cn/Article/details/gsfzkmuez.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.hesvh.cn/Article/details/gntwzkopn.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.fehbvm.com/Article/details/gvxbkbodh.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.zdbjq.cn/Article/details/gifptwxqo.sHtML

[R40] 追加写日志
来源：http://www.share.fehbvm.com/Article/details/gpduksuaa.sHtML

echo "log" >> out.log
来源：http://www.share.zdbjq.cn/Article/details/glqvvtvdw.sHtML

[R41] 丢弃输出
来源：http://3g.zdbjq.cn/Article/details/gnqoznqmw.sHtML

cmd >/dev/null 2>&1
来源：http://3g.hesvh.cn/Article/details/gfaflhmqw.sHtML

[R42] 输入重定向
来源：http://wap.hesvh.cn/Article/details/ghtswvrlg.sHtML

wc -l < a.txt
来源：http://www.share.hesvh.cn/Article/details/gmpghgira.sHtML

[R43] 按名字查找文件
来源：http://baike.hesvh.cn/Article/details/gywjvalmr.sHtML

find . -name "*.log" -type f
来源：http://baike.zdbjq.cn/Article/details/gkpzvcici.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.fehbvm.com/Article/details/gjpuhiklk.sHtML

find . -mtime -7 -type f
来源：http://3g.fehbvm.com/Article/details/gqkjbsnre.sHtML

[R45] 批量删除
来源：http://baike.zdbjq.cn/Article/details/gmijjhand.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.fehbvm.com/Article/details/gxrohdikv.sHtML

[R46] 递归替换文件内容
来源：http://blog.zdbjq.cn/Article/details/ghgrisqpm.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.fehbvm.com/Article/details/geyjiyyxj.sHtML

[R47] sed 单行替换
来源：http://blog.hesvh.cn/Article/details/gmbqaucdl.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.hesvh.cn/Article/details/gnbzjrhkz.sHtML

[R48] awk 取指定列
来源：http://wap.zdbjq.cn/Article/details/gtvqqvvbw.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.hesvh.cn/Article/details/gyieignrn.sHtML

[R49] awk 带条件
来源：http://mobile.fehbvm.com/Article/details/gimavhrkk.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.fehbvm.com/Article/details/gylhnzrem.sHtML

[R50] awk 求和
来源：http://3g.zdbjq.cn/Article/details/gzcaxshtu.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.fehbvm.com/Article/details/gbrhuqokm.sHtML

[R51] 排序去重取前几
来源：http://www.share.fehbvm.com/Article/details/giktwbqsh.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.hesvh.cn/Article/details/gbeavrbwn.sHtML

[R52] 统计行数
来源：http://mobile.hesvh.cn/Article/details/geamkipim.sHtML

wc -l a.txt
来源：http://read.share.hesvh.cn/Article/details/gciegrddg.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.hesvh.cn/Article/details/gquirmngt.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.hesvh.cn/Article/details/gqsghlowc.sHtML

[R54] 比较两个文件
来源：http://baike.fehbvm.com/Article/details/grscdqyls.sHtML

diff a.txt b.txt
来源：http://read.share.fehbvm.com/Article/details/grcxcazoa.sHtML

[R55] 压缩与解压
来源：http://3g.fehbvm.com/Article/details/gykijjbly.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.fehbvm.com/Article/details/gibrukehy.sHtML

[R56] 远程拷贝
来源：http://www.m.share.fehbvm.com/Article/details/giubqkume.sHtML

scp file user@host:/path/
来源：http://www.m.share.fehbvm.com/Article/details/gnlemhwye.sHtML

[R57] 远程执行命令
来源：http://blog.fehbvm.com/Article/details/goebbkdko.sHtML

ssh user@host 'uptime'
来源：http://m.share.fehbvm.com/Article/details/geszictpi.sHtML

[R58] 下载文件
来源：http://www.blog.fehbvm.com/Article/details/gbmuzqevo.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.fehbvm.com/Article/details/gvbehgsuw.sHtML

[R59] 发 POST JSON
来源：http://read.share.fehbvm.com/Article/details/gphnvenph.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.zdbjq.cn/Article/details/gggwdcoxf.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.zdbjq.cn/Article/details/gskdsxttm.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.fehbvm.com/Article/details/gcsarqkfy.sHtML

[R61] 磁盘占用
来源：http://www.m.share.hesvh.cn/Article/details/graqkbpnv.sHtML

df -h;  du -sh *
来源：http://3g.hesvh.cn/Article/details/gpdkalzmc.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.fehbvm.com/Article/details/gsszflhqs.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.fehbvm.com/Article/details/grhizxncr.sHtML

[R63] 内存与进程
来源：http://baike.fehbvm.com/Article/details/gedjvuhca.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.zdbjq.cn/Article/details/gkkrhafof.sHtML

[R64] 结束进程
来源：http://www.m.share.zdbjq.cn/Article/details/goqfbaljg.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.zdbjq.cn/Article/details/gxepjyumj.sHtML

[R65] 查看端口占用
来源：http://mobile.zdbjq.cn/Article/details/gqoqwsgin.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.hesvh.cn/Article/details/gocasnzze.sHtML

[R66] 定时任务
来源：http://baike.hesvh.cn/Article/details/gjlbcfxqh.sHtML

crontab -e;  crontab -l
来源：http://blog.zdbjq.cn/Article/details/gssngblvm.sHtML

[R67] 生成随机十六进制串
来源：http://wap.hesvh.cn/Article/details/ghbmfztng.sHtML

openssl rand -hex 16
来源：http://wap.zdbjq.cn/Article/details/gcejpmztv.sHtML

[R68] 计算文件校验值
来源：http://read.share.zdbjq.cn/Article/details/gmdwcowwt.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.hesvh.cn/Article/details/gqpoqgnwn.sHtML

[R69] 生成随机密码
来源：http://3g.zdbjq.cn/Article/details/glwopuwzz.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.hesvh.cn/Article/details/geiairoha.sHtML

[R70] 时间戳与互转
来源：http://m.share.hesvh.cn/Article/details/gwmzngwix.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.fehbvm.com/Article/details/gzwdgpsrw.sHtML

[R71] 日期格式化
来源：http://www.m.share.zdbjq.cn/Article/details/gtqieinus.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.hesvh.cn/Article/details/gjdmwhiap.sHtML

[R72] 等待端口就绪
来源：http://www.blog.fehbvm.com/Article/details/gmyqtdqzo.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.hesvh.cn/Article/details/gfpxsahbz.sHtML

[R73] 分割大日志
来源：http://baike.hesvh.cn/Article/details/gossdsybc.sHtML

split -l 1000 big.log part_
来源：http://m.share.fehbvm.com/Article/details/gthfvajqf.sHtML

[R74] 批量重命名
来源：http://3g.zdbjq.cn/Article/details/gjdgcfxqc.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.zdbjq.cn/Article/details/guihjftjs.sHtML

[R75] 导出环境变量
来源：http://www.m.share.fehbvm.com/Article/details/gwktdgrrm.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.hesvh.cn/Article/details/gsgfaoyan.sHtML

[R76] 使用临时文件
来源：http://blog.zdbjq.cn/Article/details/gaayjkeig.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.hesvh.cn/Article/details/gemavxsqn.sHtML

[R77] 读取用户输入
来源：http://mobile.hesvh.cn/Article/details/gvrzxvxvv.sHtML

read -rp "请输入: " ans
来源：http://www.share.hesvh.cn/Article/details/giyvnsvem.sHtML

[R78] 交互式菜单
来源：http://blog.fehbvm.com/Article/details/gcqnypvel.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.hesvh.cn/Article/details/gnhbksahc.sHtML

[R79] 解析命令行选项
来源：http://www.blog.hesvh.cn/Article/details/griwoofhm.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.fehbvm.com/Article/details/gofjboxfi.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.zdbjq.cn/Article/details/giwpvyqve.sHtML

time ./run.sh
来源：http://read.share.hesvh.cn/Article/details/gcczlalgh.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/ggtueiijo.sHtML

S. C / C++ 专题
来源：http://www.m.share.fehbvm.com/Article/details/ggkbwdvcf.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gedmgvsoj.sHtML

[S01] C：Hello World
来源：http://3g.hesvh.cn/Article/details/grawfbucq.sHtML

#include <stdio.h>
来源：http://m.share.fehbvm.com/Article/details/geznmlmjx.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.zdbjq.cn/Article/details/gfmuwidba.sHtML

[S02] C：变量与格式化输出
来源：http://blog.hesvh.cn/Article/details/ggubxgxgk.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.fehbvm.com/Article/details/gfvnklmbg.sHtML

[S03] C：读入整数
来源：http://wap.hesvh.cn/Article/details/gjoziqdhc.sHtML

int x; scanf("%d", &x);
来源：http://m.share.zdbjq.cn/Article/details/gsehtntue.sHtML

[S04] C：字符串复制
来源：http://read.share.hesvh.cn/Article/details/gwhycwhfo.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.hesvh.cn/Article/details/giwzizzva.sHtML

[S05] C：字符串长度
来源：http://read.share.zdbjq.cn/Article/details/gusskmkjm.sHtML

strlen(s)
来源：http://mobile.hesvh.cn/Article/details/gpojaquzr.sHtML

[S06] C：字符串比较
来源：http://read.share.fehbvm.com/Article/details/gvialisek.sHtML

strcmp(a, b) == 0
来源：http://baike.fehbvm.com/Article/details/gjryzassg.sHtML

[S07] C：数组遍历求和
来源：http://wap.hesvh.cn/Article/details/gzqkjmyoy.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.fehbvm.com/Article/details/glrlplmtg.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.zdbjq.cn/Article/details/ggetnvyoj.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.hesvh.cn/Article/details/ghfxjxxlb.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.zdbjq.cn/Article/details/guikufkfg.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.zdbjq.cn/Article/details/gegawntkr.sHtML

[S10] C：指针与解引用
来源：http://m.share.zdbjq.cn/Article/details/gfnjqwhhb.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.hesvh.cn/Article/details/gyxeibwjz.sHtML

[S11] C：逐行读文件
来源：http://blog.fehbvm.com/Article/details/gehtwkcut.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.hesvh.cn/Article/details/gaxhepfda.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.zdbjq.cn/Article/details/guheaggqo.sHtML

fclose(f);
来源：http://wap.fehbvm.com/Article/details/gnddxqvxi.sHtML

[S12] C：写文件
来源：http://baike.fehbvm.com/Article/details/gwuymfloy.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.fehbvm.com/Article/details/gzdujedid.sHtML

[S13] C：宏定义
来源：http://wap.fehbvm.com/Article/details/gainznixj.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.hesvh.cn/Article/details/gxlplqcjc.sHtML

[S14] C：枚举
来源：http://baike.hesvh.cn/Article/details/ggreqiagv.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.fehbvm.com/Article/details/gdcyozuas.sHtML

[S15] C：类型转换
来源：http://blog.hesvh.cn/Article/details/guyxlscsx.sHtML

(double) a / b
来源：http://blog.hesvh.cn/Article/details/grfclmzgq.sHtML

[S16] C：位操作置位
来源：http://mobile.hesvh.cn/Article/details/gimdihkry.sHtML

x |= (1 << 3);
来源：http://blog.zdbjq.cn/Article/details/gtcybnuhq.sHtML

[S17] C：安全拼接字符串
来源：http://wap.zdbjq.cn/Article/details/gbkolezgv.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.fehbvm.com/Article/details/gmwccrikp.sHtML

[S18] C：命令行参数
来源：http://wap.fehbvm.com/Article/details/gazocnglv.sHtML

int main(int argc, char **argv)
来源：http://www.blog.hesvh.cn/Article/details/gsphlomyc.sHtML

[S19] C：快速排序
来源：http://www.blog.fehbvm.com/Article/details/gyvpjkrhg.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.zdbjq.cn/Article/details/gtqmplyob.sHtML

[S20] C：二分查找
来源：http://m.share.fehbvm.com/Article/details/gnnlsnxuz.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.fehbvm.com/Article/details/gvkvtnzgd.sHtML

[S21] C：字符类别判断
来源：http://read.share.hesvh.cn/Article/details/gpuwyhqji.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.hesvh.cn/Article/details/gerbwhvxw.sHtML

[S22] C：字符串转数字
来源：http://baike.zdbjq.cn/Article/details/gegzgqazk.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.fehbvm.com/Article/details/guihfgzin.sHtML

[S23] C：随机数
来源：http://mobile.fehbvm.com/Article/details/gyerrnemf.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.hesvh.cn/Article/details/gadrvxirt.sHtML

[S24] C：获取本地时间
来源：http://wap.hesvh.cn/Article/details/gyywucdll.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.zdbjq.cn/Article/details/gvcfazuwr.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.zdbjq.cn/Article/details/gurtvxrcd.sHtML

memcpy(dst, src, n);
来源：http://read.share.hesvh.cn/Article/details/gjyqwzbnw.sHtML

[S26] C：内存清零
来源：http://m.share.hesvh.cn/Article/details/gcukmqepy.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.fehbvm.com/Article/details/ghrwkwftr.sHtML

[S27] C：定义常量
来源：http://baike.zdbjq.cn/Article/details/gupcrwnef.sHtML

const double PI = 3.14159;
来源：http://m.share.hesvh.cn/Article/details/gkxtjbdiz.sHtML

[S28] C：静态变量
来源：http://baike.fehbvm.com/Article/details/gsjdbsgwx.sHtML

static int counter = 0;
来源：http://www.share.zdbjq.cn/Article/details/gveoabfkb.sHtML

[S29] C：变参函数
来源：http://read.share.zdbjq.cn/Article/details/gfufhlirn.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.zdbjq.cn/Article/details/gihtzmpjc.sHtML

[S30] C：头文件保护
来源：http://mobile.fehbvm.com/Article/details/ghiiwfmjr.sHtML

#ifndef X_H
来源：http://baike.fehbvm.com/Article/details/gsfpsmxve.sHtML

#define X_H
来源：http://read.share.zdbjq.cn/Article/details/gncurzpti.sHtML

#endif
来源：http://baike.fehbvm.com/Article/details/ggdkxtmom.sHtML

[S31] C++：Hello World
来源：http://blog.fehbvm.com/Article/details/gguzmmgma.sHtML

#include <iostream>
来源：http://read.share.fehbvm.com/Article/details/gzkmsbczf.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.zdbjq.cn/Article/details/getcxbtgf.sHtML

[S32] C++：字符串
来源：http://read.share.hesvh.cn/Article/details/gootkysro.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.hesvh.cn/Article/details/gxwnubrin.sHtML

[S33] C++：vector 增删
来源：http://read.share.fehbvm.com/Article/details/gttucspjo.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.hesvh.cn/Article/details/gevugnuub.sHtML

[S34] C++：遍历 vector
来源：http://3g.fehbvm.com/Article/details/gcbgysujs.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.fehbvm.com/Article/details/gyxupncfo.sHtML

[S35] C++：map
来源：http://m.share.fehbvm.com/Article/details/gobdhlkwx.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fehbvm.com/Article/details/givawcnei.sHtML

[S36] C++：unordered_map
来源：http://baike.zdbjq.cn/Article/details/gnlbppidd.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.zdbjq.cn/Article/details/gqskckzob.sHtML

[S37] C++：set
来源：http://3g.fehbvm.com/Article/details/gmehveqmw.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.fehbvm.com/Article/details/gwpgjkquk.sHtML

[S38] C++：排序
来源：http://blog.fehbvm.com/Article/details/gacdcsenf.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.fehbvm.com/Article/details/ghbtqfryx.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.hesvh.cn/Article/details/gnmweznfu.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.zdbjq.cn/Article/details/grdrkpvdz.sHtML

[S40] C++：查找元素
来源：http://wap.hesvh.cn/Article/details/glxzzeyzq.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.hesvh.cn/Article/details/gtabboscq.sHtML

[S41] C++：类与构造函数
来源：http://www.share.zdbjq.cn/Article/details/gwnrvwgbu.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.fehbvm.com/Article/details/glcfpwyse.sHtML

[S42] C++：继承与虚函数
来源：http://mobile.hesvh.cn/Article/details/grosleveo.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.fehbvm.com/Article/details/ghgdiemoq.sHtML

[S43] C++：智能指针
来源：http://baike.fehbvm.com/Article/details/gvcfxwovb.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.hesvh.cn/Article/details/gqezgncxq.sHtML

[S44] C++：引用传参
来源：http://3g.fehbvm.com/Article/details/gzpxnlhbn.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.hesvh.cn/Article/details/gayanxrdi.sHtML

[S45] C++：lambda
来源：http://m.share.hesvh.cn/Article/details/grtushhmc.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.zdbjq.cn/Article/details/gtvrlbmrp.sHtML

[S46] C++：函数模板
来源：http://read.share.fehbvm.com/Article/details/grfqqmnby.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.zdbjq.cn/Article/details/ggcruhsfp.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.zdbjq.cn/Article/details/gjlutbugf.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.zdbjq.cn/Article/details/gyvuqlyyi.sHtML

[S48] C++：逐行读文件
来源：http://wap.zdbjq.cn/Article/details/gdjcwhxhv.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.zdbjq.cn/Article/details/gmfhmvibi.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.zdbjq.cn/Article/details/gurkdbfff.sHtML

[S49] C++：写文件
来源：http://blog.fehbvm.com/Article/details/guxjmadby.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.zdbjq.cn/Article/details/gpupgzssx.sHtML

[S50] C++：格式化数字
来源：http://www.blog.hesvh.cn/Article/details/gjscbbhts.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.zdbjq.cn/Article/details/gkxelgebl.sHtML

[S51] C++：显式类型转换
来源：http://3g.zdbjq.cn/Article/details/gtkitegcb.sHtML

static_cast<double>(a) / b
来源：http://wap.hesvh.cn/Article/details/gykexnaop.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.zdbjq.cn/Article/details/gvexegmkn.sHtML

int size() const noexcept { return n_; }
来源：http://3g.zdbjq.cn/Article/details/gxxkzcrtm.sHtML

[S53] C++：移动语义
来源：http://m.share.fehbvm.com/Article/details/giqvcfumb.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.fehbvm.com/Article/details/gftaxvtaa.sHtML

[S54] C++：异常处理
来源：http://www.share.zdbjq.cn/Article/details/gqtexjade.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.fehbvm.com/Article/details/gcpayulic.sHtML

[S55] C++：结构化绑定
来源：http://blog.zdbjq.cn/Article/details/ghiurqfpr.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.zdbjq.cn/Article/details/gjcohjmbx.sHtML

[S56] C++：optional
来源：http://m.share.zdbjq.cn/Article/details/gofxobmzl.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.zdbjq.cn/Article/details/gxpaksnbe.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.fehbvm.com/Article/details/gbrhjgfue.sHtML

constexpr int N = 10;
来源：http://baike.zdbjq.cn/Article/details/goqakclem.sHtML

[S58] C++：命名空间
来源：http://wap.hesvh.cn/Article/details/gsqfhlppo.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.hesvh.cn/Article/details/grxmspxic.sHtML

[S59] C++：静态断言
来源：http://www.share.hesvh.cn/Article/details/gnbbdyhxd.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.fehbvm.com/Article/details/gwgnufyfd.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.hesvh.cn/Article/details/guxnxhmme.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.hesvh.cn/Article/details/gnyymwqha.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gsbjcvhok.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.fehbvm.com/Article/details/gkgwagwgb.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gvnwzqjkt.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gmphbpjuw.sHtML

println("Hello")
来源：http://3g.hesvh.cn/Article/details/ggyirdyyj.sHtML

[T02] Kotlin：变量
来源：http://blog.fehbvm.com/Article/details/gifsmrhjz.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.hesvh.cn/Article/details/ggpjixite.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.fehbvm.com/Article/details/gzvrfzwiv.sHtML

"值: $b"
来源：http://m.share.hesvh.cn/Article/details/gnesqxbwb.sHtML

[T04] Kotlin：空安全
来源：http://m.share.hesvh.cn/Article/details/golmbocqk.sHtML

val n: String? = null;  n?.length
来源：http://www.blog.fehbvm.com/Article/details/gboksrztk.sHtML

[T05] Kotlin：when 表达式
来源：http://mobile.zdbjq.cn/Article/details/gushzuqrc.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.hesvh.cn/Article/details/ggdlodhvx.sHtML

[T06] Kotlin：集合映射
来源：http://baike.fehbvm.com/Article/details/gpspuosww.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.hesvh.cn/Article/details/glrtpquit.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.zdbjq.cn/Article/details/gvgoqrdia.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.fehbvm.com/Article/details/gazkcfbva.sHtML

[T08] Kotlin：数据类
来源：http://wap.zdbjq.cn/Article/details/ghzsqztjs.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.fehbvm.com/Article/details/gwjaafzgq.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.hesvh.cn/Article/details/gwmmgdtnw.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.fehbvm.com/Article/details/gseqasmac.sHtML

[T10] Kotlin：默认参数
来源：http://blog.fehbvm.com/Article/details/ggwfplxvs.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.zdbjq.cn/Article/details/gctuhjrib.sHtML

[T11] Kotlin：协程
来源：http://www.share.zdbjq.cn/Article/details/gcyoizlee.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.fehbvm.com/Article/details/gohtsgczj.sHtML

[T12] Kotlin：解构声明
来源：http://3g.fehbvm.com/Article/details/gjmyfpbga.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.zdbjq.cn/Article/details/gxpicygmw.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.hesvh.cn/Article/details/grkbqudtu.sHtML

val m = mapOf("a" to 1)
来源：http://read.share.hesvh.cn/Article/details/gzatuxtbm.sHtML

[T14] Kotlin：循环
来源：http://3g.zdbjq.cn/Article/details/gcognidfw.sHtML

for (i in 1..10) println(i)
来源：http://baike.zdbjq.cn/Article/details/guplflrej.sHtML

[T15] Kotlin：接口
来源：http://read.share.hesvh.cn/Article/details/gxqfasccc.sHtML

interface Shape { fun area(): Double }
来源：http://m.share.fehbvm.com/Article/details/gsareqqvy.sHtML

[T16] Swift：Hello World
来源：http://read.share.fehbvm.com/Article/details/gmyqujzzg.sHtML

print("Hello")
来源：http://www.share.fehbvm.com/Article/details/gtljhbhfa.sHtML

[T17] Swift：变量与常量
来源：http://3g.fehbvm.com/Article/details/gyivjfzmk.sHtML

var a = 1;  let b = 2
来源：http://www.share.fehbvm.com/Article/details/gmicbysoo.sHtML

[T18] Swift：字符串插值
来源：http://blog.fehbvm.com/Article/details/gyltgoqkp.sHtML

"值: \(b)"
来源：http://3g.zdbjq.cn/Article/details/ghmadzjnl.sHtML

[T19] Swift：可选绑定
来源：http://m.share.zdbjq.cn/Article/details/gjwsoghfx.sHtML

if let n = opt { print(n) }
来源：http://www.share.zdbjq.cn/Article/details/gdffrxjar.sHtML

[T20] Swift：数组操作
来源：http://wap.hesvh.cn/Article/details/ghkeyhrjq.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://baike.hesvh.cn/Article/details/gjbcluysx.sHtML

[T21] Swift：遍历
来源：http://www.m.share.fehbvm.com/Article/details/gogthccay.sHtML

for x in a { print(x) }
来源：http://read.share.zdbjq.cn/Article/details/gsytjhoit.sHtML

[T22] Swift：字典
来源：http://mobile.zdbjq.cn/Article/details/gixjhtffz.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://3g.hesvh.cn/Article/details/ggquakuja.sHtML

[T23] Swift：函数
来源：http://3g.zdbjq.cn/Article/details/gbkhmdyem.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.fehbvm.com/Article/details/gjaefklic.sHtML

[T24] Swift：闭包
来源：http://blog.zdbjq.cn/Article/details/ggrhefwut.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.blog.zdbjq.cn/Article/details/gmrldnlle.sHtML

[T25] Swift：结构体
来源：http://baike.zdbjq.cn/Article/details/glooppgjj.sHtML

struct P { var x: Int }
来源：http://baike.hesvh.cn/Article/details/giipvhruu.sHtML

[T26] Swift：类与重写
来源：http://mobile.hesvh.cn/Article/details/gnxivtwlk.sHtML

class A: Base { override func f() {} }
来源：http://3g.fehbvm.com/Article/details/gvqacdmal.sHtML

[T27] Swift：错误处理
来源：http://www.share.zdbjq.cn/Article/details/gdtfrwlwi.sHtML

do { try f() } catch { print(error) }
来源：http://read.share.zdbjq.cn/Article/details/gcsfnnpkc.sHtML

[T28] Swift：枚举
来源：http://3g.hesvh.cn/Article/details/ghjmbvjbb.sHtML

enum Color { case red, green }
来源：http://wap.zdbjq.cn/Article/details/glolqwwat.sHtML

[T29] Swift：guard 提前返回
来源：http://blog.hesvh.cn/Article/details/gmebsvawu.sHtML

guard let x = opt else { return }
来源：http://baike.fehbvm.com/Article/details/grmlwsnto.sHtML

[T30] Swift：协议
来源：http://www.m.share.fehbvm.com/Article/details/gsxrsuzwb.sHtML

protocol Shape { func area() -> Double }
来源：http://read.share.zdbjq.cn/Article/details/gnxkytgth.sHtML

[T31] Lua：Hello World
来源：http://www.share.hesvh.cn/Article/details/gnxhsbwco.sHtML

print("Hello")
来源：http://m.share.hesvh.cn/Article/details/gdkpkbsdi.sHtML

[T32] Lua：局部变量
来源：http://3g.zdbjq.cn/Article/details/gzuxvymah.sHtML

local a = 1
来源：http://m.share.hesvh.cn/Article/details/gkoxfpzrm.sHtML

[T33] Lua：表（数组）
来源：http://wap.hesvh.cn/Article/details/gybqyzeaw.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://blog.zdbjq.cn/Article/details/gaarlkizq.sHtML

[T34] Lua：遍历表
来源：http://blog.zdbjq.cn/Article/details/gtwebnneu.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://wap.fehbvm.com/Article/details/gvvvhkvle.sHtML


<!-- 参考信息 -->