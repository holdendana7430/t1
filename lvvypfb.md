代发 wailian999

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.fehbvm.com/Article/details/grabruuqq.sHtML

[R30] 函数返回状态码
来源：http://wap.fehbvm.com/Article/details/gxxsenclg.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.hesvh.cn/Article/details/gwqhyootk.sHtML

[R31] 局部变量
来源：http://3g.fehbvm.com/Article/details/gdzporagx.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.fehbvm.com/Article/details/guotoumpm.sHtML

[R32] 参数个数校验
来源：http://m.share.hesvh.cn/Article/details/gzdksgrrj.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.hesvh.cn/Article/details/gjchrxozl.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.hesvh.cn/Article/details/glhqvqeqo.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.hesvh.cn/Article/details/gwicvfusq.sHtML

[R34] 退出时清理
来源：http://read.share.zdbjq.cn/Article/details/ggzvfojqe.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.hesvh.cn/Article/details/gkbyehtth.sHtML

[R35] 后台执行并等待
来源：http://baike.fehbvm.com/Article/details/gtivkbpak.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.hesvh.cn/Article/details/gcfiwdkgi.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.fehbvm.com/Article/details/gupfdbevx.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.hesvh.cn/Article/details/gpqfdcmde.sHtML

[R37] 把输出赋给变量
来源：http://m.share.zdbjq.cn/Article/details/gpbpxaqyx.sHtML

files=$(ls -1)
来源：http://blog.zdbjq.cn/Article/details/giwsrkinh.sHtML

[R38] 管道串联
来源：http://read.share.fehbvm.com/Article/details/gzjoemrnf.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.zdbjq.cn/Article/details/gqwqaeizn.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.fehbvm.com/Article/details/gjffdbcau.sHtML

cmd > out.log 2>&1
来源：http://mobile.hesvh.cn/Article/details/gdpxayedj.sHtML

[R40] 追加写日志
来源：http://www.blog.fehbvm.com/Article/details/gjwtibbab.sHtML

echo "log" >> out.log
来源：http://www.share.fehbvm.com/Article/details/gdacmelvx.sHtML

[R41] 丢弃输出
来源：http://wap.hesvh.cn/Article/details/gqsorkzqg.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.zdbjq.cn/Article/details/gywwugmlt.sHtML

[R42] 输入重定向
来源：http://m.share.fehbvm.com/Article/details/ghvedzhyp.sHtML

wc -l < a.txt
来源：http://blog.hesvh.cn/Article/details/gnxdygcvb.sHtML

[R43] 按名字查找文件
来源：http://mobile.zdbjq.cn/Article/details/gjjktpxpn.sHtML

find . -name "*.log" -type f
来源：http://3g.zdbjq.cn/Article/details/gdupwqdjz.sHtML

[R44] 按修改时间查找
来源：http://baike.fehbvm.com/Article/details/gslppgkpi.sHtML

find . -mtime -7 -type f
来源：http://m.share.zdbjq.cn/Article/details/glnvtbivq.sHtML

[R45] 批量删除
来源：http://www.blog.fehbvm.com/Article/details/glkxhmbfr.sHtML

find . -name "*.tmp" -delete
来源：http://wap.fehbvm.com/Article/details/ghnhtmpbc.sHtML

[R46] 递归替换文件内容
来源：http://blog.hesvh.cn/Article/details/gshhbewzx.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.fehbvm.com/Article/details/gxadagxhu.sHtML

[R47] sed 单行替换
来源：http://read.share.hesvh.cn/Article/details/gqyxpxbkl.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.hesvh.cn/Article/details/gekbgndou.sHtML

[R48] awk 取指定列
来源：http://mobile.hesvh.cn/Article/details/gwbvkqkxh.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.hesvh.cn/Article/details/gjzlhweqn.sHtML

[R49] awk 带条件
来源：http://read.share.zdbjq.cn/Article/details/glkfytirw.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.zdbjq.cn/Article/details/gvzovdvqc.sHtML

[R50] awk 求和
来源：http://3g.zdbjq.cn/Article/details/gqwjlgnfy.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.zdbjq.cn/Article/details/gwrigdkgk.sHtML

[R51] 排序去重取前几
来源：http://www.blog.hesvh.cn/Article/details/gujzizlom.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.zdbjq.cn/Article/details/glnjvysfk.sHtML

[R52] 统计行数
来源：http://www.m.share.fehbvm.com/Article/details/grnzwrdsv.sHtML

wc -l a.txt
来源：http://www.share.zdbjq.cn/Article/details/gfjngccip.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.zdbjq.cn/Article/details/gboukbumr.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.fehbvm.com/Article/details/gpsxazlkc.sHtML

[R54] 比较两个文件
来源：http://mobile.fehbvm.com/Article/details/ghvpecono.sHtML

diff a.txt b.txt
来源：http://www.share.hesvh.cn/Article/details/gvjshhtwc.sHtML

[R55] 压缩与解压
来源：http://read.share.fehbvm.com/Article/details/gfyzuzkel.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.zdbjq.cn/Article/details/guusvkaph.sHtML

[R56] 远程拷贝
来源：http://blog.zdbjq.cn/Article/details/gkpdzcfap.sHtML

scp file user@host:/path/
来源：http://www.m.share.zdbjq.cn/Article/details/gjjjirdkt.sHtML

[R57] 远程执行命令
来源：http://www.share.fehbvm.com/Article/details/gletfhlbj.sHtML

ssh user@host 'uptime'
来源：http://mobile.fehbvm.com/Article/details/gepnogjep.sHtML

[R58] 下载文件
来源：http://www.blog.fehbvm.com/Article/details/gvkxihmbk.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.fehbvm.com/Article/details/gaxjimold.sHtML

[R59] 发 POST JSON
来源：http://wap.zdbjq.cn/Article/details/grjgzmzuf.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.fehbvm.com/Article/details/gebfmvqzi.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.zdbjq.cn/Article/details/gsclnpnsu.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.fehbvm.com/Article/details/gftpthdsu.sHtML

[R61] 磁盘占用
来源：http://blog.fehbvm.com/Article/details/gzclicldp.sHtML

df -h;  du -sh *
来源：http://read.share.hesvh.cn/Article/details/gclkxjzkz.sHtML

[R62] 找最占空间的文件
来源：http://mobile.fehbvm.com/Article/details/ggkuvjaya.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.hesvh.cn/Article/details/grewwipin.sHtML

[R63] 内存与进程
来源：http://wap.zdbjq.cn/Article/details/gfrgwxwsa.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.zdbjq.cn/Article/details/gmzpcbmby.sHtML

[R64] 结束进程
来源：http://3g.fehbvm.com/Article/details/ggtssygvz.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.hesvh.cn/Article/details/gsvzfsvrb.sHtML

[R65] 查看端口占用
来源：http://read.share.fehbvm.com/Article/details/gxdyxwpmk.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.zdbjq.cn/Article/details/gutsndycn.sHtML

[R66] 定时任务
来源：http://m.share.zdbjq.cn/Article/details/gjxhtfzdc.sHtML

crontab -e;  crontab -l
来源：http://blog.fehbvm.com/Article/details/gauueeszy.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.fehbvm.com/Article/details/gwtunxrzm.sHtML

openssl rand -hex 16
来源：http://mobile.hesvh.cn/Article/details/gqplujzrv.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.zdbjq.cn/Article/details/gajpioyca.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/glirpktov.sHtML

[R69] 生成随机密码
来源：http://3g.hesvh.cn/Article/details/gqnoiojan.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.fehbvm.com/Article/details/ghgnekdmf.sHtML

[R70] 时间戳与互转
来源：http://read.share.hesvh.cn/Article/details/gyeqngudq.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.fehbvm.com/Article/details/ghbguawbf.sHtML

[R71] 日期格式化
来源：http://m.share.hesvh.cn/Article/details/gxottiwzv.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://read.share.hesvh.cn/Article/details/gtpmabniu.sHtML

[R72] 等待端口就绪
来源：http://www.blog.fehbvm.com/Article/details/gfaxppqpl.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.fehbvm.com/Article/details/gvfzvdbpp.sHtML

[R73] 分割大日志
来源：http://www.m.share.hesvh.cn/Article/details/guwquqamq.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.hesvh.cn/Article/details/glgdpfngd.sHtML

[R74] 批量重命名
来源：http://blog.fehbvm.com/Article/details/gzgvbezcv.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.hesvh.cn/Article/details/gmcqexgzb.sHtML

[R75] 导出环境变量
来源：http://www.m.share.fehbvm.com/Article/details/gpmztsgbd.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.fehbvm.com/Article/details/gajrechdx.sHtML

[R76] 使用临时文件
来源：http://wap.fehbvm.com/Article/details/ghoyecbyz.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.hesvh.cn/Article/details/ggfatlsly.sHtML

[R77] 读取用户输入
来源：http://www.blog.fehbvm.com/Article/details/guhqtqobd.sHtML

read -rp "请输入: " ans
来源：http://baike.fehbvm.com/Article/details/gbmzsoabh.sHtML

[R78] 交互式菜单
来源：http://m.share.hesvh.cn/Article/details/gtjxwmkbw.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.zdbjq.cn/Article/details/gxaxnwvge.sHtML

[R79] 解析命令行选项
来源：http://wap.zdbjq.cn/Article/details/gzfwlrrfc.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.fehbvm.com/Article/details/gjjsxmfsk.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.fehbvm.com/Article/details/gdkpclkrl.sHtML

time ./run.sh
来源：http://wap.hesvh.cn/Article/details/gchpgmzfy.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gcuaqubec.sHtML

S. C / C++ 专题
来源：http://m.share.fehbvm.com/Article/details/ghtqcqtbd.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/guqtpoptf.sHtML

[S01] C：Hello World
来源：http://wap.zdbjq.cn/Article/details/gnrgplmsm.sHtML

#include <stdio.h>
来源：http://www.share.fehbvm.com/Article/details/giprrtnte.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.fehbvm.com/Article/details/gpzhreort.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.hesvh.cn/Article/details/gczccwwfd.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.hesvh.cn/Article/details/gzygnqqwl.sHtML

[S03] C：读入整数
来源：http://3g.hesvh.cn/Article/details/gfufmxryi.sHtML

int x; scanf("%d", &x);
来源：http://wap.zdbjq.cn/Article/details/glltgxqfj.sHtML

[S04] C：字符串复制
来源：http://read.share.hesvh.cn/Article/details/glcvpozwy.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.zdbjq.cn/Article/details/gzpcsjmup.sHtML

[S05] C：字符串长度
来源：http://www.blog.zdbjq.cn/Article/details/gbdcqyxqj.sHtML

strlen(s)
来源：http://wap.fehbvm.com/Article/details/glntmehjg.sHtML

[S06] C：字符串比较
来源：http://mobile.zdbjq.cn/Article/details/gvazrhlvl.sHtML

strcmp(a, b) == 0
来源：http://m.share.hesvh.cn/Article/details/gkcfmhexd.sHtML

[S07] C：数组遍历求和
来源：http://3g.fehbvm.com/Article/details/gaywqtnms.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.zdbjq.cn/Article/details/gdamtsyyq.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.fehbvm.com/Article/details/gfvwxoyyc.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.hesvh.cn/Article/details/girlwapbq.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.zdbjq.cn/Article/details/grmfolsps.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.hesvh.cn/Article/details/gufiwtvin.sHtML

[S10] C：指针与解引用
来源：http://www.share.zdbjq.cn/Article/details/gvxctzvnj.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.hesvh.cn/Article/details/ggmcfrdtc.sHtML

[S11] C：逐行读文件
来源：http://3g.zdbjq.cn/Article/details/girpytvlr.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.hesvh.cn/Article/details/gzeprxptu.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.hesvh.cn/Article/details/gweznyfjj.sHtML

fclose(f);
来源：http://read.share.fehbvm.com/Article/details/gjkuuytfb.sHtML

[S12] C：写文件
来源：http://www.m.share.fehbvm.com/Article/details/gfdttvfvj.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.fehbvm.com/Article/details/gctaifupy.sHtML

[S13] C：宏定义
来源：http://www.blog.zdbjq.cn/Article/details/gomubdhap.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.hesvh.cn/Article/details/gmqiqmwcc.sHtML

[S14] C：枚举
来源：http://baike.hesvh.cn/Article/details/glplmdnnz.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.hesvh.cn/Article/details/gsdvktgqs.sHtML

[S15] C：类型转换
来源：http://www.share.fehbvm.com/Article/details/gmxaryjsj.sHtML

(double) a / b
来源：http://wap.hesvh.cn/Article/details/gycvgtkcb.sHtML

[S16] C：位操作置位
来源：http://www.blog.zdbjq.cn/Article/details/ghjfvutyc.sHtML

x |= (1 << 3);
来源：http://m.share.fehbvm.com/Article/details/gatfqzlxm.sHtML

[S17] C：安全拼接字符串
来源：http://blog.hesvh.cn/Article/details/gaixuxmrj.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.hesvh.cn/Article/details/gmhvfvori.sHtML

[S18] C：命令行参数
来源：http://blog.hesvh.cn/Article/details/gpdyjnsvb.sHtML

int main(int argc, char **argv)
来源：http://baike.fehbvm.com/Article/details/gyhvskvkh.sHtML

[S19] C：快速排序
来源：http://www.share.zdbjq.cn/Article/details/gdkkuuclu.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.hesvh.cn/Article/details/grflzwuun.sHtML

[S20] C：二分查找
来源：http://m.share.hesvh.cn/Article/details/ghmpbqwmg.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.fehbvm.com/Article/details/getwrjmdd.sHtML

[S21] C：字符类别判断
来源：http://blog.zdbjq.cn/Article/details/gathkquqv.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.fehbvm.com/Article/details/gxvybebpz.sHtML

[S22] C：字符串转数字
来源：http://read.share.fehbvm.com/Article/details/gjuoefrkm.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.zdbjq.cn/Article/details/gahilytuz.sHtML

[S23] C：随机数
来源：http://baike.fehbvm.com/Article/details/gdcdpaquc.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.hesvh.cn/Article/details/gcckxwqdg.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.hesvh.cn/Article/details/gbjfzilvw.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.fehbvm.com/Article/details/gwneicmgu.sHtML

[S25] C：内存拷贝
来源：http://blog.zdbjq.cn/Article/details/gccuyadtf.sHtML

memcpy(dst, src, n);
来源：http://read.share.fehbvm.com/Article/details/ggtbjzkbr.sHtML

[S26] C：内存清零
来源：http://www.m.share.hesvh.cn/Article/details/gwbwbqmgk.sHtML

memset(a, 0, sizeof a);
来源：http://blog.fehbvm.com/Article/details/gawogqmjt.sHtML

[S27] C：定义常量
来源：http://www.m.share.hesvh.cn/Article/details/gmldiwrrq.sHtML

const double PI = 3.14159;
来源：http://3g.zdbjq.cn/Article/details/gfylgeeoh.sHtML

[S28] C：静态变量
来源：http://www.blog.fehbvm.com/Article/details/ggeblmfdl.sHtML

static int counter = 0;
来源：http://www.m.share.fehbvm.com/Article/details/gokrvskzu.sHtML

[S29] C：变参函数
来源：http://read.share.zdbjq.cn/Article/details/gqlmjjxkg.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.fehbvm.com/Article/details/gpfjpbvrx.sHtML

[S30] C：头文件保护
来源：http://www.m.share.hesvh.cn/Article/details/gflfppjhc.sHtML

#ifndef X_H
来源：http://read.share.hesvh.cn/Article/details/ggpctsscv.sHtML

#define X_H
来源：http://baike.fehbvm.com/Article/details/gtkokjgal.sHtML

#endif
来源：http://wap.zdbjq.cn/Article/details/gboihexkd.sHtML

[S31] C++：Hello World
来源：http://blog.fehbvm.com/Article/details/gazykpkpw.sHtML

#include <iostream>
来源：http://m.share.hesvh.cn/Article/details/gharkvmqa.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.hesvh.cn/Article/details/gktwajayz.sHtML

[S32] C++：字符串
来源：http://www.blog.zdbjq.cn/Article/details/gsncgpxhs.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.fehbvm.com/Article/details/gdibaccxi.sHtML

[S33] C++：vector 增删
来源：http://mobile.fehbvm.com/Article/details/gpxzbekzz.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.fehbvm.com/Article/details/gxirnxhmx.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.fehbvm.com/Article/details/gvncfdbcj.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.zdbjq.cn/Article/details/gvhiklifp.sHtML

[S35] C++：map
来源：http://mobile.hesvh.cn/Article/details/gnafnposi.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.fehbvm.com/Article/details/gmlnahgrq.sHtML

[S36] C++：unordered_map
来源：http://baike.zdbjq.cn/Article/details/gewmawnri.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.zdbjq.cn/Article/details/gcynbnwns.sHtML

[S37] C++：set
来源：http://m.share.zdbjq.cn/Article/details/gyqvciydo.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.fehbvm.com/Article/details/gsvfijsor.sHtML

[S38] C++：排序
来源：http://wap.hesvh.cn/Article/details/gpeqnroaw.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.zdbjq.cn/Article/details/gkhwxvuwr.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.zdbjq.cn/Article/details/gmkhojnvh.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.fehbvm.com/Article/details/gchvtvfqx.sHtML

[S40] C++：查找元素
来源：http://m.share.zdbjq.cn/Article/details/grwpnntjn.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.zdbjq.cn/Article/details/gphceaopa.sHtML

[S41] C++：类与构造函数
来源：http://baike.zdbjq.cn/Article/details/gwzercikx.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.hesvh.cn/Article/details/geexhbgsk.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.hesvh.cn/Article/details/gscnowwox.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.zdbjq.cn/Article/details/gdybocxor.sHtML

[S43] C++：智能指针
来源：http://m.share.zdbjq.cn/Article/details/gqwckraaf.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.zdbjq.cn/Article/details/gtufdwmiy.sHtML

[S44] C++：引用传参
来源：http://wap.fehbvm.com/Article/details/ghkzxvqny.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.hesvh.cn/Article/details/glxftyxrb.sHtML

[S45] C++：lambda
来源：http://www.blog.zdbjq.cn/Article/details/grmyygwwv.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.hesvh.cn/Article/details/gndebtynp.sHtML

[S46] C++：函数模板
来源：http://www.blog.hesvh.cn/Article/details/gojorkdkk.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.hesvh.cn/Article/details/ggeihtlpv.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.hesvh.cn/Article/details/geuvmcplo.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.zdbjq.cn/Article/details/gcunvafqx.sHtML

[S48] C++：逐行读文件
来源：http://blog.fehbvm.com/Article/details/gkdtxbnlx.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://m.share.fehbvm.com/Article/details/gvrfbsmlx.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.zdbjq.cn/Article/details/goeuajiim.sHtML

[S49] C++：写文件
来源：http://baike.hesvh.cn/Article/details/gbdcqrmik.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.fehbvm.com/Article/details/gafqiuaed.sHtML

[S50] C++：格式化数字
来源：http://www.share.hesvh.cn/Article/details/gpnpenljc.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.zdbjq.cn/Article/details/gaypomkeh.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.hesvh.cn/Article/details/gssxvcjvk.sHtML

static_cast<double>(a) / b
来源：http://www.blog.hesvh.cn/Article/details/gfgzfgnzx.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.fehbvm.com/Article/details/gruqnjyiq.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.hesvh.cn/Article/details/grqbhfkyl.sHtML

[S53] C++：移动语义
来源：http://3g.fehbvm.com/Article/details/gvlkyjkfe.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.hesvh.cn/Article/details/gfgisbcqo.sHtML

[S54] C++：异常处理
来源：http://3g.zdbjq.cn/Article/details/gwhyclgjj.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.hesvh.cn/Article/details/grnyxblcl.sHtML

[S55] C++：结构化绑定
来源：http://read.share.fehbvm.com/Article/details/gqwguiwic.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.fehbvm.com/Article/details/gvjuqttjb.sHtML

[S56] C++：optional
来源：http://www.blog.zdbjq.cn/Article/details/giihuvuml.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.zdbjq.cn/Article/details/glsgowvoq.sHtML

[S57] C++：编译期常量
来源：http://m.share.hesvh.cn/Article/details/gnpwpdrbi.sHtML

constexpr int N = 10;
来源：http://read.share.fehbvm.com/Article/details/gjusnpweu.sHtML

[S58] C++：命名空间
来源：http://blog.zdbjq.cn/Article/details/gwlhkmviu.sHtML

namespace ns { int f() { return 1; } }
来源：http://blog.zdbjq.cn/Article/details/gpkujcrhf.sHtML

[S59] C++：静态断言
来源：http://www.blog.hesvh.cn/Article/details/glgfuevrv.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.zdbjq.cn/Article/details/gapteqxmj.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.fehbvm.com/Article/details/ghkrijmdz.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.fehbvm.com/Article/details/gcakjfatk.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/grsnwtrmn.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.fehbvm.com/Article/details/gqzyvrudi.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/guonrtgtr.sHtML

[T01] Kotlin：Hello World
来源：http://wap.hesvh.cn/Article/details/gtjcadavq.sHtML

println("Hello")
来源：http://wap.fehbvm.com/Article/details/goluaxhpp.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.fehbvm.com/Article/details/gdrdqkbfn.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.zdbjq.cn/Article/details/guayvwtjx.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.fehbvm.com/Article/details/guncfdlwt.sHtML

"值: $b"
来源：http://m.share.hesvh.cn/Article/details/gtegqwdei.sHtML

[T04] Kotlin：空安全
来源：http://mobile.zdbjq.cn/Article/details/gxvjvtqct.sHtML

val n: String? = null;  n?.length
来源：http://m.share.zdbjq.cn/Article/details/gajpdnmmu.sHtML

[T05] Kotlin：when 表达式
来源：http://mobile.hesvh.cn/Article/details/gupsfieap.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.hesvh.cn/Article/details/gyyurgchq.sHtML

[T06] Kotlin：集合映射
来源：http://blog.zdbjq.cn/Article/details/gcmqtnibs.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.zdbjq.cn/Article/details/gphzeixrl.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.zdbjq.cn/Article/details/gepvsjeha.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://baike.fehbvm.com/Article/details/guvvbpbba.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.fehbvm.com/Article/details/gqsvnekbq.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.zdbjq.cn/Article/details/gcurnovwl.sHtML

[T09] Kotlin：扩展函数
来源：http://mobile.zdbjq.cn/Article/details/grvmtsvfn.sHtML

fun String.exclaim() = this + "!"
来源：http://blog.fehbvm.com/Article/details/gmvcilieb.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.fehbvm.com/Article/details/gnnqnqbbl.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.hesvh.cn/Article/details/gfmmjaknb.sHtML

[T11] Kotlin：协程
来源：http://www.share.hesvh.cn/Article/details/gxvnkzljz.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.fehbvm.com/Article/details/gohkvbaak.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.fehbvm.com/Article/details/gcokrirja.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.fehbvm.com/Article/details/gvcgmpzte.sHtML

[T13] Kotlin：只读 Map
来源：http://read.share.hesvh.cn/Article/details/ghryitqtw.sHtML

val m = mapOf("a" to 1)
来源：http://wap.hesvh.cn/Article/details/gyanynbmv.sHtML

[T14] Kotlin：循环
来源：http://mobile.zdbjq.cn/Article/details/gyideuwlh.sHtML

for (i in 1..10) println(i)
来源：http://mobile.zdbjq.cn/Article/details/gejzcdivu.sHtML

[T15] Kotlin：接口
来源：http://www.share.zdbjq.cn/Article/details/gsgrgexrc.sHtML

interface Shape { fun area(): Double }
来源：http://wap.zdbjq.cn/Article/details/ggsjhbnib.sHtML

[T16] Swift：Hello World
来源：http://m.share.hesvh.cn/Article/details/gdpxoerfl.sHtML

print("Hello")
来源：http://m.share.hesvh.cn/Article/details/guvjvwclp.sHtML

[T17] Swift：变量与常量
来源：http://mobile.zdbjq.cn/Article/details/grfohmheo.sHtML

var a = 1;  let b = 2
来源：http://m.share.zdbjq.cn/Article/details/gucyzojvm.sHtML

[T18] Swift：字符串插值
来源：http://baike.zdbjq.cn/Article/details/gtjslmkqv.sHtML

"值: \(b)"
来源：http://www.share.hesvh.cn/Article/details/gnebickwr.sHtML

[T19] Swift：可选绑定
来源：http://mobile.zdbjq.cn/Article/details/gjorrvxsk.sHtML

if let n = opt { print(n) }
来源：http://baike.zdbjq.cn/Article/details/gxkocrwli.sHtML

[T20] Swift：数组操作
来源：http://baike.zdbjq.cn/Article/details/gpdomgbea.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://mobile.hesvh.cn/Article/details/gfnqocirf.sHtML

[T21] Swift：遍历
来源：http://blog.fehbvm.com/Article/details/gdzfhxxam.sHtML

for x in a { print(x) }
来源：http://www.blog.fehbvm.com/Article/details/gyjeebwzm.sHtML

[T22] Swift：字典
来源：http://3g.fehbvm.com/Article/details/gcqfexsoh.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.blog.zdbjq.cn/Article/details/grbwzpxyq.sHtML

[T23] Swift：函数
来源：http://wap.hesvh.cn/Article/details/gvhpdynaz.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.hesvh.cn/Article/details/gucfvehce.sHtML

[T24] Swift：闭包
来源：http://wap.fehbvm.com/Article/details/gcwtscrkb.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://m.share.hesvh.cn/Article/details/gvlgixdjs.sHtML

[T25] Swift：结构体
来源：http://wap.hesvh.cn/Article/details/gwqxufvix.sHtML

struct P { var x: Int }
来源：http://baike.fehbvm.com/Article/details/glxxblocg.sHtML

[T26] Swift：类与重写
来源：http://www.blog.zdbjq.cn/Article/details/gpyrxqnza.sHtML

class A: Base { override func f() {} }
来源：http://3g.fehbvm.com/Article/details/gpzjfrvib.sHtML

[T27] Swift：错误处理
来源：http://baike.hesvh.cn/Article/details/gbppkwnyc.sHtML

do { try f() } catch { print(error) }
来源：http://blog.zdbjq.cn/Article/details/glzhqvlov.sHtML

[T28] Swift：枚举
来源：http://blog.zdbjq.cn/Article/details/gusctjkom.sHtML

enum Color { case red, green }
来源：http://www.m.share.hesvh.cn/Article/details/gdqmautmr.sHtML

[T29] Swift：guard 提前返回
来源：http://mobile.zdbjq.cn/Article/details/gzxxndnun.sHtML

guard let x = opt else { return }
来源：http://www.blog.fehbvm.com/Article/details/gylwdkpui.sHtML

[T30] Swift：协议
来源：http://3g.fehbvm.com/Article/details/gfhzyohfx.sHtML

protocol Shape { func area() -> Double }
来源：http://blog.zdbjq.cn/Article/details/gdgoxukuj.sHtML

[T31] Lua：Hello World
来源：http://read.share.hesvh.cn/Article/details/grzozmhfs.sHtML

print("Hello")
来源：http://wap.fehbvm.com/Article/details/gjpuxhkup.sHtML

[T32] Lua：局部变量
来源：http://m.share.zdbjq.cn/Article/details/gduiwzhmy.sHtML

local a = 1
来源：http://www.blog.hesvh.cn/Article/details/gfxmkdlwc.sHtML


<!-- 参考信息 -->