代发 wailian999

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.zdbjq.cn/Article/details/gpioxjvkc.sHtML

[R30] 函数返回状态码
来源：http://blog.zdbjq.cn/Article/details/gxdpjncny.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.fehbvm.com/Article/details/ghanvnkma.sHtML

[R31] 局部变量
来源：http://3g.zdbjq.cn/Article/details/gyrohshgf.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.hesvh.cn/Article/details/giwvcnpuj.sHtML

[R32] 参数个数校验
来源：http://www.m.share.hesvh.cn/Article/details/gbgwvmgoz.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.zdbjq.cn/Article/details/gopqpnppm.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.fehbvm.com/Article/details/gzjhlczth.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.zdbjq.cn/Article/details/gmizzayax.sHtML

[R34] 退出时清理
来源：http://www.share.zdbjq.cn/Article/details/gztdqhkmk.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.fehbvm.com/Article/details/ggabpuotq.sHtML

[R35] 后台执行并等待
来源：http://read.share.zdbjq.cn/Article/details/gscocawhf.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.zdbjq.cn/Article/details/glvsedfss.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.hesvh.cn/Article/details/ghgdsnyar.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.hesvh.cn/Article/details/gbaxoytwr.sHtML

[R37] 把输出赋给变量
来源：http://3g.fehbvm.com/Article/details/gtjzlgyri.sHtML

files=$(ls -1)
来源：http://wap.zdbjq.cn/Article/details/gjehdoold.sHtML

[R38] 管道串联
来源：http://www.m.share.fehbvm.com/Article/details/gfftkrbex.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.hesvh.cn/Article/details/gmfxvfxyh.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.fehbvm.com/Article/details/gjgxryhko.sHtML

cmd > out.log 2>&1
来源：http://baike.zdbjq.cn/Article/details/grxoygjlf.sHtML

[R40] 追加写日志
来源：http://mobile.zdbjq.cn/Article/details/gsvdsssow.sHtML

echo "log" >> out.log
来源：http://m.share.fehbvm.com/Article/details/gnndrhfvr.sHtML

[R41] 丢弃输出
来源：http://www.share.hesvh.cn/Article/details/ghgqizdhm.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.hesvh.cn/Article/details/gkkhahduq.sHtML

[R42] 输入重定向
来源：http://blog.zdbjq.cn/Article/details/giluwgwjf.sHtML

wc -l < a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gmywjrggu.sHtML

[R43] 按名字查找文件
来源：http://www.share.hesvh.cn/Article/details/gzzxdwerr.sHtML

find . -name "*.log" -type f
来源：http://m.share.zdbjq.cn/Article/details/grwhokijo.sHtML

[R44] 按修改时间查找
来源：http://www.blog.zdbjq.cn/Article/details/glfqfocrw.sHtML

find . -mtime -7 -type f
来源：http://wap.fehbvm.com/Article/details/gympkdvyj.sHtML

[R45] 批量删除
来源：http://blog.fehbvm.com/Article/details/gerkdyzxs.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.hesvh.cn/Article/details/gdusvcsml.sHtML

[R46] 递归替换文件内容
来源：http://m.share.hesvh.cn/Article/details/gfoackmxp.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.zdbjq.cn/Article/details/gzcaufmkv.sHtML

[R47] sed 单行替换
来源：http://3g.fehbvm.com/Article/details/gakccmlbf.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.fehbvm.com/Article/details/gzajbzmgo.sHtML

[R48] awk 取指定列
来源：http://www.blog.fehbvm.com/Article/details/gdhayfpil.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.hesvh.cn/Article/details/gsrviieds.sHtML

[R49] awk 带条件
来源：http://3g.hesvh.cn/Article/details/grqflhrrs.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.zdbjq.cn/Article/details/galacydhl.sHtML

[R50] awk 求和
来源：http://m.share.zdbjq.cn/Article/details/gwpaqryqn.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.fehbvm.com/Article/details/ggvszrvwy.sHtML

[R51] 排序去重取前几
来源：http://mobile.hesvh.cn/Article/details/gjobjvybe.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.hesvh.cn/Article/details/gpdzfvesa.sHtML

[R52] 统计行数
来源：http://baike.fehbvm.com/Article/details/gdyajcxgv.sHtML

wc -l a.txt
来源：http://www.m.share.hesvh.cn/Article/details/glinppwsx.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.fehbvm.com/Article/details/gsdpqbnor.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.zdbjq.cn/Article/details/gzavunvka.sHtML

[R54] 比较两个文件
来源：http://www.share.zdbjq.cn/Article/details/gsonacaez.sHtML

diff a.txt b.txt
来源：http://read.share.fehbvm.com/Article/details/gendigaly.sHtML

[R55] 压缩与解压
来源：http://www.share.fehbvm.com/Article/details/gofweeyuh.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.zdbjq.cn/Article/details/gbjqkxxtd.sHtML

[R56] 远程拷贝
来源：http://baike.fehbvm.com/Article/details/gjzfkjpmh.sHtML

scp file user@host:/path/
来源：http://www.share.hesvh.cn/Article/details/guvdpdpld.sHtML

[R57] 远程执行命令
来源：http://m.share.fehbvm.com/Article/details/gzhaeasyu.sHtML

ssh user@host 'uptime'
来源：http://www.share.fehbvm.com/Article/details/glnofrntl.sHtML

[R58] 下载文件
来源：http://wap.zdbjq.cn/Article/details/glkbblgrh.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.fehbvm.com/Article/details/gyhbxudtr.sHtML

[R59] 发 POST JSON
来源：http://baike.zdbjq.cn/Article/details/gzmibncfp.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.fehbvm.com/Article/details/gqjxecutl.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.zdbjq.cn/Article/details/gmdutwban.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.fehbvm.com/Article/details/goboanwnk.sHtML

[R61] 磁盘占用
来源：http://m.share.fehbvm.com/Article/details/gdlwfkikp.sHtML

df -h;  du -sh *
来源：http://blog.hesvh.cn/Article/details/gnedtpqyd.sHtML

[R62] 找最占空间的文件
来源：http://baike.zdbjq.cn/Article/details/gkvopugvi.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.zdbjq.cn/Article/details/gbyszfnvs.sHtML

[R63] 内存与进程
来源：http://blog.hesvh.cn/Article/details/gwkzhkhgp.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.zdbjq.cn/Article/details/gbodhsaog.sHtML

[R64] 结束进程
来源：http://m.share.zdbjq.cn/Article/details/gkrwyiwgj.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.fehbvm.com/Article/details/gbmcbankn.sHtML

[R65] 查看端口占用
来源：http://3g.hesvh.cn/Article/details/gzzhvcypa.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.zdbjq.cn/Article/details/glpcgqops.sHtML

[R66] 定时任务
来源：http://www.share.fehbvm.com/Article/details/glqdpxwne.sHtML

crontab -e;  crontab -l
来源：http://www.share.hesvh.cn/Article/details/gywodjxfo.sHtML

[R67] 生成随机十六进制串
来源：http://wap.fehbvm.com/Article/details/gokiuzgjd.sHtML

openssl rand -hex 16
来源：http://mobile.zdbjq.cn/Article/details/guxocrfih.sHtML

[R68] 计算文件校验值
来源：http://www.blog.fehbvm.com/Article/details/gmcohekab.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.hesvh.cn/Article/details/ghissysbe.sHtML

[R69] 生成随机密码
来源：http://mobile.zdbjq.cn/Article/details/gerwpxdek.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.zdbjq.cn/Article/details/gsodpttat.sHtML

[R70] 时间戳与互转
来源：http://baike.zdbjq.cn/Article/details/gapllvxtp.sHtML

date +%s;  date -d @1700000000
来源：http://m.share.zdbjq.cn/Article/details/gestwsjer.sHtML

[R71] 日期格式化
来源：http://mobile.zdbjq.cn/Article/details/gjsxmbbbs.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.zdbjq.cn/Article/details/gmqvqaxkv.sHtML

[R72] 等待端口就绪
来源：http://www.share.zdbjq.cn/Article/details/gwwfvnfih.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.zdbjq.cn/Article/details/gwxriqzcq.sHtML

[R73] 分割大日志
来源：http://mobile.fehbvm.com/Article/details/gutgnnuau.sHtML

split -l 1000 big.log part_
来源：http://wap.hesvh.cn/Article/details/gxigxohyn.sHtML

[R74] 批量重命名
来源：http://read.share.zdbjq.cn/Article/details/gjwxkeova.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.zdbjq.cn/Article/details/gjtvwjkia.sHtML

[R75] 导出环境变量
来源：http://read.share.hesvh.cn/Article/details/gxvoqzayq.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.zdbjq.cn/Article/details/gnxiisslb.sHtML

[R76] 使用临时文件
来源：http://m.share.hesvh.cn/Article/details/grhmkjpjj.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.hesvh.cn/Article/details/ghkknrnqw.sHtML

[R77] 读取用户输入
来源：http://baike.hesvh.cn/Article/details/gdcbpbaas.sHtML

read -rp "请输入: " ans
来源：http://3g.zdbjq.cn/Article/details/gtaqbyign.sHtML

[R78] 交互式菜单
来源：http://m.share.fehbvm.com/Article/details/gaadeqnzr.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.zdbjq.cn/Article/details/gwtylxejx.sHtML

[R79] 解析命令行选项
来源：http://m.share.zdbjq.cn/Article/details/gtxyqfwki.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.fehbvm.com/Article/details/gbcgvueow.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.zdbjq.cn/Article/details/gcwznzwrp.sHtML

time ./run.sh
来源：http://baike.zdbjq.cn/Article/details/gcazsonct.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gbpxupuag.sHtML

S. C / C++ 专题
来源：http://baike.fehbvm.com/Article/details/gonhrtgch.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gmnpyczwy.sHtML

[S01] C：Hello World
来源：http://wap.zdbjq.cn/Article/details/gcptpzskb.sHtML

#include <stdio.h>
来源：http://3g.hesvh.cn/Article/details/gfzzkupnn.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.fehbvm.com/Article/details/gofprccel.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.zdbjq.cn/Article/details/goaxuzddg.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.fehbvm.com/Article/details/gddgblzbk.sHtML

[S03] C：读入整数
来源：http://www.m.share.zdbjq.cn/Article/details/gdikrwwuu.sHtML

int x; scanf("%d", &x);
来源：http://wap.fehbvm.com/Article/details/gurxpfybu.sHtML

[S04] C：字符串复制
来源：http://www.share.fehbvm.com/Article/details/gnnvowmmy.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.hesvh.cn/Article/details/gqrdyvsaj.sHtML

[S05] C：字符串长度
来源：http://www.blog.zdbjq.cn/Article/details/gjscvewlz.sHtML

strlen(s)
来源：http://mobile.zdbjq.cn/Article/details/gmthcmmdm.sHtML

[S06] C：字符串比较
来源：http://wap.hesvh.cn/Article/details/gqbtvrzmm.sHtML

strcmp(a, b) == 0
来源：http://baike.fehbvm.com/Article/details/gduczhrfi.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.hesvh.cn/Article/details/gzlqshcbs.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.zdbjq.cn/Article/details/gtodyopyg.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.zdbjq.cn/Article/details/gdzupvbba.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.hesvh.cn/Article/details/gcreujpjf.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.fehbvm.com/Article/details/gaqvpwwka.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.zdbjq.cn/Article/details/gernosqzm.sHtML

[S10] C：指针与解引用
来源：http://www.blog.fehbvm.com/Article/details/gskfmqhzx.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.zdbjq.cn/Article/details/gtgtuoswp.sHtML

[S11] C：逐行读文件
来源：http://www.share.hesvh.cn/Article/details/gducgtmfr.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.zdbjq.cn/Article/details/gjswggtni.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.hesvh.cn/Article/details/guiccbtce.sHtML

fclose(f);
来源：http://m.share.fehbvm.com/Article/details/gsslvljue.sHtML

[S12] C：写文件
来源：http://wap.hesvh.cn/Article/details/gqaznuylr.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.hesvh.cn/Article/details/glrzprvba.sHtML

[S13] C：宏定义
来源：http://www.share.hesvh.cn/Article/details/gpdiklwsp.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.fehbvm.com/Article/details/gxmqftaen.sHtML

[S14] C：枚举
来源：http://blog.hesvh.cn/Article/details/gxxevagpp.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.zdbjq.cn/Article/details/gnrezrdds.sHtML

[S15] C：类型转换
来源：http://3g.hesvh.cn/Article/details/gskuifnio.sHtML

(double) a / b
来源：http://read.share.zdbjq.cn/Article/details/gqmcbdckj.sHtML

[S16] C：位操作置位
来源：http://m.share.zdbjq.cn/Article/details/ggbvtrnuc.sHtML

x |= (1 << 3);
来源：http://mobile.fehbvm.com/Article/details/gclkqmsus.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.zdbjq.cn/Article/details/gultpouuy.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.fehbvm.com/Article/details/gxqersrkw.sHtML

[S18] C：命令行参数
来源：http://www.m.share.zdbjq.cn/Article/details/gmyzddwmp.sHtML

int main(int argc, char **argv)
来源：http://blog.fehbvm.com/Article/details/gvryygrsw.sHtML

[S19] C：快速排序
来源：http://www.m.share.fehbvm.com/Article/details/gafxavgjw.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.hesvh.cn/Article/details/gxfhovdju.sHtML

[S20] C：二分查找
来源：http://www.blog.fehbvm.com/Article/details/gsylhnvha.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.zdbjq.cn/Article/details/gbkdbniuy.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.fehbvm.com/Article/details/gldlnwkcg.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.zdbjq.cn/Article/details/gkbkymfzm.sHtML

[S22] C：字符串转数字
来源：http://read.share.zdbjq.cn/Article/details/glzrsywjo.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.hesvh.cn/Article/details/ggjtxkvvf.sHtML

[S23] C：随机数
来源：http://3g.hesvh.cn/Article/details/ggautemuj.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.fehbvm.com/Article/details/gscfjnhgb.sHtML

[S24] C：获取本地时间
来源：http://m.share.hesvh.cn/Article/details/gtnbtpzlb.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.hesvh.cn/Article/details/grmjobern.sHtML

[S25] C：内存拷贝
来源：http://www.share.zdbjq.cn/Article/details/gtludjgwp.sHtML

memcpy(dst, src, n);
来源：http://blog.fehbvm.com/Article/details/gmunvxrml.sHtML

[S26] C：内存清零
来源：http://www.m.share.zdbjq.cn/Article/details/gvoftanfh.sHtML

memset(a, 0, sizeof a);
来源：http://baike.hesvh.cn/Article/details/guzysirsh.sHtML

[S27] C：定义常量
来源：http://www.share.fehbvm.com/Article/details/gdajnrbtt.sHtML

const double PI = 3.14159;
来源：http://3g.hesvh.cn/Article/details/gfxrscimp.sHtML

[S28] C：静态变量
来源：http://www.m.share.hesvh.cn/Article/details/gkipwtrft.sHtML

static int counter = 0;
来源：http://blog.fehbvm.com/Article/details/gtgngyobm.sHtML

[S29] C：变参函数
来源：http://www.blog.hesvh.cn/Article/details/gcosfgurb.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.zdbjq.cn/Article/details/gtewcwxuz.sHtML

[S30] C：头文件保护
来源：http://baike.zdbjq.cn/Article/details/gtxfmqqdu.sHtML

#ifndef X_H
来源：http://www.m.share.fehbvm.com/Article/details/gmqkzpaoz.sHtML

#define X_H
来源：http://www.blog.zdbjq.cn/Article/details/gcyiprclm.sHtML

#endif
来源：http://wap.hesvh.cn/Article/details/gjojyfbtj.sHtML

[S31] C++：Hello World
来源：http://read.share.fehbvm.com/Article/details/gpnfpvjro.sHtML

#include <iostream>
来源：http://www.m.share.zdbjq.cn/Article/details/gadshlchk.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.hesvh.cn/Article/details/gwsvfqtyl.sHtML

[S32] C++：字符串
来源：http://3g.hesvh.cn/Article/details/gawszayls.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.fehbvm.com/Article/details/givpdysec.sHtML

[S33] C++：vector 增删
来源：http://3g.fehbvm.com/Article/details/gvqqthmom.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.zdbjq.cn/Article/details/gvxytljlk.sHtML

[S34] C++：遍历 vector
来源：http://mobile.fehbvm.com/Article/details/gnyqfzbtl.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.hesvh.cn/Article/details/gfjcyjavq.sHtML

[S35] C++：map
来源：http://3g.hesvh.cn/Article/details/gpfrfcebu.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fehbvm.com/Article/details/gilrzuiev.sHtML

[S36] C++：unordered_map
来源：http://mobile.hesvh.cn/Article/details/goycbbxag.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.hesvh.cn/Article/details/ghpdthzgq.sHtML

[S37] C++：set
来源：http://www.blog.fehbvm.com/Article/details/goyaquaxn.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.fehbvm.com/Article/details/ghfxgocaf.sHtML

[S38] C++：排序
来源：http://3g.fehbvm.com/Article/details/gvgnlvwoz.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.fehbvm.com/Article/details/ggjwyxdhe.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.zdbjq.cn/Article/details/gbhyzjihk.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.hesvh.cn/Article/details/gmlytrfdm.sHtML

[S40] C++：查找元素
来源：http://wap.hesvh.cn/Article/details/gsavsxyri.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.fehbvm.com/Article/details/gbqjvuvfm.sHtML

[S41] C++：类与构造函数
来源：http://blog.fehbvm.com/Article/details/ghtuquevd.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.hesvh.cn/Article/details/gwdiomicq.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.fehbvm.com/Article/details/gmnjodsoq.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.fehbvm.com/Article/details/geodgyygr.sHtML

[S43] C++：智能指针
来源：http://read.share.zdbjq.cn/Article/details/grttmrbwe.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.zdbjq.cn/Article/details/ghdkqkbrt.sHtML

[S44] C++：引用传参
来源：http://read.share.fehbvm.com/Article/details/gsbtitjtg.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.fehbvm.com/Article/details/gtwevxnaf.sHtML

[S45] C++：lambda
来源：http://mobile.fehbvm.com/Article/details/googxscjj.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.zdbjq.cn/Article/details/gngxqukat.sHtML

[S46] C++：函数模板
来源：http://mobile.fehbvm.com/Article/details/ggvzyfnnd.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.zdbjq.cn/Article/details/gmkhvwewv.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.zdbjq.cn/Article/details/gsignoapu.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.hesvh.cn/Article/details/gxpkfhisu.sHtML

[S48] C++：逐行读文件
来源：http://3g.fehbvm.com/Article/details/gelfqblot.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.hesvh.cn/Article/details/gkbchxahw.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.zdbjq.cn/Article/details/gaezbocwb.sHtML

[S49] C++：写文件
来源：http://www.share.hesvh.cn/Article/details/guibfxock.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.fehbvm.com/Article/details/gsqphheni.sHtML

[S50] C++：格式化数字
来源：http://www.blog.zdbjq.cn/Article/details/ggecsoyld.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.hesvh.cn/Article/details/gucpymlnm.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.zdbjq.cn/Article/details/gplpxigdj.sHtML

static_cast<double>(a) / b
来源：http://wap.fehbvm.com/Article/details/gwlnekxuw.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.hesvh.cn/Article/details/gcfziovfl.sHtML

int size() const noexcept { return n_; }
来源：http://blog.fehbvm.com/Article/details/gsjgbolru.sHtML

[S53] C++：移动语义
来源：http://baike.fehbvm.com/Article/details/gsrqmtohb.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.zdbjq.cn/Article/details/gabbviiol.sHtML

[S54] C++：异常处理
来源：http://www.blog.zdbjq.cn/Article/details/gblyphcvu.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.hesvh.cn/Article/details/gwfkqbtle.sHtML

[S55] C++：结构化绑定
来源：http://read.share.zdbjq.cn/Article/details/ghxvfrfge.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.zdbjq.cn/Article/details/gmpnokkwp.sHtML

[S56] C++：optional
来源：http://blog.fehbvm.com/Article/details/gdexnyozf.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.zdbjq.cn/Article/details/gygehgkbb.sHtML

[S57] C++：编译期常量
来源：http://baike.hesvh.cn/Article/details/gxcoohwqb.sHtML

constexpr int N = 10;
来源：http://baike.hesvh.cn/Article/details/ggvhyyfgf.sHtML

[S58] C++：命名空间
来源：http://baike.hesvh.cn/Article/details/gcpvinvpo.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.hesvh.cn/Article/details/gllqbhknk.sHtML

[S59] C++：静态断言
来源：http://www.share.hesvh.cn/Article/details/gdbxahech.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.zdbjq.cn/Article/details/gmbiwozig.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.zdbjq.cn/Article/details/guegxvjyp.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.fehbvm.com/Article/details/gectvcgoc.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gnpudxioy.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.fehbvm.com/Article/details/gxbpviuqa.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gkyiiualm.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.hesvh.cn/Article/details/gfgvfivtv.sHtML

println("Hello")
来源：http://read.share.hesvh.cn/Article/details/gszbdmanl.sHtML

[T02] Kotlin：变量
来源：http://blog.hesvh.cn/Article/details/gpdlurnuu.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.fehbvm.com/Article/details/gqitpfsoz.sHtML

[T03] Kotlin：字符串模板
来源：http://www.m.share.hesvh.cn/Article/details/gntxlqaqa.sHtML

"值: $b"
来源：http://3g.zdbjq.cn/Article/details/getmodwsd.sHtML

[T04] Kotlin：空安全
来源：http://mobile.hesvh.cn/Article/details/gnoknhjzp.sHtML

val n: String? = null;  n?.length
来源：http://mobile.fehbvm.com/Article/details/gcifyxqjo.sHtML

[T05] Kotlin：when 表达式
来源：http://mobile.hesvh.cn/Article/details/gbqetfhqb.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://read.share.hesvh.cn/Article/details/gnnxilxyb.sHtML

[T06] Kotlin：集合映射
来源：http://wap.hesvh.cn/Article/details/gubetwofj.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.fehbvm.com/Article/details/gzchgsgul.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.hesvh.cn/Article/details/gozpswfyy.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.fehbvm.com/Article/details/gwrqwqvpd.sHtML

[T08] Kotlin：数据类
来源：http://www.share.fehbvm.com/Article/details/grchlbrwf.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.fehbvm.com/Article/details/grdfltuji.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.hesvh.cn/Article/details/gwxlqyfsq.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.hesvh.cn/Article/details/gdfhhkywo.sHtML

[T10] Kotlin：默认参数
来源：http://blog.zdbjq.cn/Article/details/gurrcokft.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.m.share.fehbvm.com/Article/details/gswsaptrp.sHtML

[T11] Kotlin：协程
来源：http://blog.fehbvm.com/Article/details/gklvxohgi.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.share.hesvh.cn/Article/details/ggxnpctfh.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.hesvh.cn/Article/details/gdnqqbwci.sHtML

val (a, b) = Pair(1, 2)
来源：http://m.share.fehbvm.com/Article/details/gpmmrpjoj.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.hesvh.cn/Article/details/gpfancujv.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.fehbvm.com/Article/details/gvtuihdac.sHtML

[T14] Kotlin：循环
来源：http://www.blog.fehbvm.com/Article/details/gvrruyibd.sHtML

for (i in 1..10) println(i)
来源：http://www.m.share.zdbjq.cn/Article/details/gcqervgok.sHtML

[T15] Kotlin：接口
来源：http://3g.hesvh.cn/Article/details/gszobpgsj.sHtML

interface Shape { fun area(): Double }
来源：http://www.m.share.hesvh.cn/Article/details/gkxbifufg.sHtML

[T16] Swift：Hello World
来源：http://m.share.hesvh.cn/Article/details/gwiekdijc.sHtML

print("Hello")
来源：http://3g.zdbjq.cn/Article/details/glywyplva.sHtML

[T17] Swift：变量与常量
来源：http://read.share.zdbjq.cn/Article/details/gcpmqikbb.sHtML

var a = 1;  let b = 2
来源：http://www.blog.fehbvm.com/Article/details/gytdhmjsb.sHtML

[T18] Swift：字符串插值
来源：http://www.m.share.fehbvm.com/Article/details/gpmdhcjyp.sHtML

"值: \(b)"
来源：http://3g.fehbvm.com/Article/details/gkxinrucw.sHtML

[T19] Swift：可选绑定
来源：http://baike.hesvh.cn/Article/details/gcoyfxsxe.sHtML

if let n = opt { print(n) }
来源：http://read.share.hesvh.cn/Article/details/gyggusrlp.sHtML

[T20] Swift：数组操作
来源：http://wap.zdbjq.cn/Article/details/getztvipw.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://m.share.zdbjq.cn/Article/details/gnjjhcmzo.sHtML

[T21] Swift：遍历
来源：http://mobile.fehbvm.com/Article/details/gybroeyas.sHtML

for x in a { print(x) }
来源：http://baike.fehbvm.com/Article/details/gmiypvclq.sHtML

[T22] Swift：字典
来源：http://read.share.fehbvm.com/Article/details/gdbapzpoy.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://baike.hesvh.cn/Article/details/gvgsyzwbl.sHtML

[T23] Swift：函数
来源：http://m.share.hesvh.cn/Article/details/geyzesvaz.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://read.share.fehbvm.com/Article/details/glxtbobff.sHtML

[T24] Swift：闭包
来源：http://baike.hesvh.cn/Article/details/gqgtjgvij.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.m.share.hesvh.cn/Article/details/gttwfgmfp.sHtML

[T25] Swift：结构体
来源：http://www.blog.hesvh.cn/Article/details/gwyixobrz.sHtML

struct P { var x: Int }
来源：http://baike.zdbjq.cn/Article/details/gmovrqahk.sHtML

[T26] Swift：类与重写
来源：http://www.blog.hesvh.cn/Article/details/gpdefyhez.sHtML

class A: Base { override func f() {} }
来源：http://www.blog.hesvh.cn/Article/details/gddyebmkb.sHtML

[T27] Swift：错误处理
来源：http://3g.fehbvm.com/Article/details/gufsqkmke.sHtML

do { try f() } catch { print(error) }
来源：http://blog.hesvh.cn/Article/details/gohsszqia.sHtML

[T28] Swift：枚举
来源：http://www.blog.hesvh.cn/Article/details/gzbmavybs.sHtML

enum Color { case red, green }
来源：http://www.share.zdbjq.cn/Article/details/gfklrabqq.sHtML

[T29] Swift：guard 提前返回
来源：http://mobile.fehbvm.com/Article/details/ginefkmwd.sHtML

guard let x = opt else { return }
来源：http://mobile.fehbvm.com/Article/details/gastbgpbd.sHtML

[T30] Swift：协议
来源：http://m.share.hesvh.cn/Article/details/gthpvjskf.sHtML

protocol Shape { func area() -> Double }
来源：http://m.share.fehbvm.com/Article/details/gmpnurdtp.sHtML

[T31] Lua：Hello World
来源：http://mobile.fehbvm.com/Article/details/gnnsauiju.sHtML

print("Hello")
来源：http://www.blog.fehbvm.com/Article/details/gtqolprow.sHtML

[T32] Lua：局部变量
来源：http://m.share.hesvh.cn/Article/details/guyinlogr.sHtML

local a = 1
来源：http://read.share.zdbjq.cn/Article/details/ghtlscoem.sHtML


<!-- 参考信息 -->