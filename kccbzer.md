代发 wailian999

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.zdbjq.cn/Article/details/gzrrwosqp.sHtML

[R30] 函数返回状态码
来源：http://blog.zdbjq.cn/Article/details/gjrtofipy.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.hesvh.cn/Article/details/gunsqhmuv.sHtML

[R31] 局部变量
来源：http://3g.zdbjq.cn/Article/details/gjzhrgzas.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.zdbjq.cn/Article/details/giadpzwjv.sHtML

[R32] 参数个数校验
来源：http://baike.fehbvm.com/Article/details/gowgvvfdg.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.fehbvm.com/Article/details/gsuycfwwk.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.fehbvm.com/Article/details/gddvowllt.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.hesvh.cn/Article/details/gubhyfgoz.sHtML

[R34] 退出时清理
来源：http://blog.zdbjq.cn/Article/details/gahycqzcu.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.hesvh.cn/Article/details/gmgacrnyh.sHtML

[R35] 后台执行并等待
来源：http://baike.fehbvm.com/Article/details/gspzgeadt.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.zdbjq.cn/Article/details/gxdhckswk.sHtML

[R36] 并发执行多个任务
来源：http://wap.fehbvm.com/Article/details/gxqpfzbsg.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.hesvh.cn/Article/details/glerybfba.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.zdbjq.cn/Article/details/gkukmpkzr.sHtML

files=$(ls -1)
来源：http://www.blog.fehbvm.com/Article/details/goyqgbvyl.sHtML

[R38] 管道串联
来源：http://blog.hesvh.cn/Article/details/gwiszmfjn.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.fehbvm.com/Article/details/glklzswds.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.zdbjq.cn/Article/details/gkqtqkkis.sHtML

cmd > out.log 2>&1
来源：http://blog.fehbvm.com/Article/details/gsmqfezfy.sHtML

[R40] 追加写日志
来源：http://blog.hesvh.cn/Article/details/ghmrzxkue.sHtML

echo "log" >> out.log
来源：http://read.share.fehbvm.com/Article/details/ghjqoinzf.sHtML

[R41] 丢弃输出
来源：http://www.m.share.zdbjq.cn/Article/details/gzvuvisqy.sHtML

cmd >/dev/null 2>&1
来源：http://blog.zdbjq.cn/Article/details/gqbixfrmh.sHtML

[R42] 输入重定向
来源：http://wap.zdbjq.cn/Article/details/ghqdosckg.sHtML

wc -l < a.txt
来源：http://m.share.fehbvm.com/Article/details/gxrvwyeej.sHtML

[R43] 按名字查找文件
来源：http://www.blog.hesvh.cn/Article/details/gztkogzrs.sHtML

find . -name "*.log" -type f
来源：http://3g.zdbjq.cn/Article/details/gedrvptyv.sHtML

[R44] 按修改时间查找
来源：http://www.share.zdbjq.cn/Article/details/gdmlxzynw.sHtML

find . -mtime -7 -type f
来源：http://read.share.fehbvm.com/Article/details/gckkoepvn.sHtML

[R45] 批量删除
来源：http://wap.fehbvm.com/Article/details/gpzubeztq.sHtML

find . -name "*.tmp" -delete
来源：http://3g.fehbvm.com/Article/details/ganqpocqh.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.hesvh.cn/Article/details/gnwmcfabw.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.zdbjq.cn/Article/details/gxccqznmu.sHtML

[R47] sed 单行替换
来源：http://www.blog.hesvh.cn/Article/details/gfglbfmtq.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.zdbjq.cn/Article/details/gqbahtice.sHtML

[R48] awk 取指定列
来源：http://blog.hesvh.cn/Article/details/ghdepetdc.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.hesvh.cn/Article/details/gflogxaqp.sHtML

[R49] awk 带条件
来源：http://3g.zdbjq.cn/Article/details/gkwotgmue.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.zdbjq.cn/Article/details/gjljedgyq.sHtML

[R50] awk 求和
来源：http://3g.hesvh.cn/Article/details/gkhelhjyu.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://blog.zdbjq.cn/Article/details/gpcsizexk.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.zdbjq.cn/Article/details/gecgovmat.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.zdbjq.cn/Article/details/gvetmijxl.sHtML

[R52] 统计行数
来源：http://www.share.zdbjq.cn/Article/details/gypsjrjfx.sHtML

wc -l a.txt
来源：http://mobile.zdbjq.cn/Article/details/gtamnzhti.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.zdbjq.cn/Article/details/gniqzgnfs.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.fehbvm.com/Article/details/gobqbfqas.sHtML

[R54] 比较两个文件
来源：http://wap.zdbjq.cn/Article/details/geqnfmctg.sHtML

diff a.txt b.txt
来源：http://blog.zdbjq.cn/Article/details/gxdxvmmcv.sHtML

[R55] 压缩与解压
来源：http://read.share.fehbvm.com/Article/details/gfgbvdyan.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.hesvh.cn/Article/details/gjqvbscal.sHtML

[R56] 远程拷贝
来源：http://mobile.fehbvm.com/Article/details/gjfivwlba.sHtML

scp file user@host:/path/
来源：http://baike.hesvh.cn/Article/details/grbxodprf.sHtML

[R57] 远程执行命令
来源：http://3g.fehbvm.com/Article/details/giyagzhvn.sHtML

ssh user@host 'uptime'
来源：http://wap.hesvh.cn/Article/details/gazbqaljh.sHtML

[R58] 下载文件
来源：http://blog.hesvh.cn/Article/details/gbnbahigl.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.hesvh.cn/Article/details/gfjdlhvxj.sHtML

[R59] 发 POST JSON
来源：http://3g.fehbvm.com/Article/details/gbgfbvnav.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.fehbvm.com/Article/details/glepnxlxt.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.fehbvm.com/Article/details/gsxjalhnu.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.zdbjq.cn/Article/details/guomvuwdz.sHtML

[R61] 磁盘占用
来源：http://mobile.fehbvm.com/Article/details/gvlzrsece.sHtML

df -h;  du -sh *
来源：http://baike.fehbvm.com/Article/details/gciwdqyms.sHtML

[R62] 找最占空间的文件
来源：http://3g.hesvh.cn/Article/details/ghywmnvba.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.zdbjq.cn/Article/details/gtlotpekr.sHtML

[R63] 内存与进程
来源：http://read.share.hesvh.cn/Article/details/gxtpblglm.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.fehbvm.com/Article/details/gwzibwtzj.sHtML

[R64] 结束进程
来源：http://www.m.share.hesvh.cn/Article/details/glspzabrf.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.hesvh.cn/Article/details/ggccyqnuj.sHtML

[R65] 查看端口占用
来源：http://www.blog.fehbvm.com/Article/details/gyuxkoecm.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.zdbjq.cn/Article/details/gjatgvcul.sHtML

[R66] 定时任务
来源：http://baike.zdbjq.cn/Article/details/gxvttpecf.sHtML

crontab -e;  crontab -l
来源：http://blog.zdbjq.cn/Article/details/gwowchivg.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.hesvh.cn/Article/details/gaxplyyjz.sHtML

openssl rand -hex 16
来源：http://read.share.fehbvm.com/Article/details/gfqvsxxrm.sHtML

[R68] 计算文件校验值
来源：http://3g.fehbvm.com/Article/details/gfftpswqw.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.zdbjq.cn/Article/details/gzoedgxjs.sHtML

[R69] 生成随机密码
来源：http://blog.hesvh.cn/Article/details/gnwocajnh.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.hesvh.cn/Article/details/gbnzgqlyy.sHtML

[R70] 时间戳与互转
来源：http://3g.hesvh.cn/Article/details/gymrrpivg.sHtML

date +%s;  date -d @1700000000
来源：http://blog.fehbvm.com/Article/details/grczvxfmt.sHtML

[R71] 日期格式化
来源：http://3g.zdbjq.cn/Article/details/gagixcwch.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.hesvh.cn/Article/details/gxxrvyufu.sHtML

[R72] 等待端口就绪
来源：http://mobile.fehbvm.com/Article/details/gskuvlabt.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.hesvh.cn/Article/details/gblundyvn.sHtML

[R73] 分割大日志
来源：http://blog.zdbjq.cn/Article/details/gjmsjgfru.sHtML

split -l 1000 big.log part_
来源：http://read.share.zdbjq.cn/Article/details/gdhqkogpa.sHtML

[R74] 批量重命名
来源：http://baike.fehbvm.com/Article/details/gxgxrgrjz.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.fehbvm.com/Article/details/gadmujkwm.sHtML

[R75] 导出环境变量
来源：http://www.share.fehbvm.com/Article/details/gvdmknxrx.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.hesvh.cn/Article/details/gawsvahbl.sHtML

[R76] 使用临时文件
来源：http://www.share.zdbjq.cn/Article/details/gglfhkfbo.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.hesvh.cn/Article/details/ghjzoepgt.sHtML

[R77] 读取用户输入
来源：http://www.share.fehbvm.com/Article/details/gbvgemglv.sHtML

read -rp "请输入: " ans
来源：http://mobile.fehbvm.com/Article/details/gewhtkhiz.sHtML

[R78] 交互式菜单
来源：http://www.m.share.hesvh.cn/Article/details/gublsthvf.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.zdbjq.cn/Article/details/gzcvybiuw.sHtML

[R79] 解析命令行选项
来源：http://www.share.hesvh.cn/Article/details/gjmopdpcg.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.fehbvm.com/Article/details/gfmzqtsdu.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.fehbvm.com/Article/details/gczuzbkye.sHtML

time ./run.sh
来源：http://www.share.zdbjq.cn/Article/details/guecwqiet.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/grygwykxl.sHtML

S. C / C++ 专题
来源：http://blog.zdbjq.cn/Article/details/gellffmnx.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gmpazdqls.sHtML

[S01] C：Hello World
来源：http://mobile.hesvh.cn/Article/details/grymvgcpy.sHtML

#include <stdio.h>
来源：http://baike.hesvh.cn/Article/details/ggrzkyhcp.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.fehbvm.com/Article/details/gaawpsgag.sHtML

[S02] C：变量与格式化输出
来源：http://blog.zdbjq.cn/Article/details/gfqakrzbp.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.hesvh.cn/Article/details/gtjlkxqnh.sHtML

[S03] C：读入整数
来源：http://3g.fehbvm.com/Article/details/ggjlixcyp.sHtML

int x; scanf("%d", &x);
来源：http://wap.hesvh.cn/Article/details/grrgrfyss.sHtML

[S04] C：字符串复制
来源：http://www.m.share.fehbvm.com/Article/details/guflceayb.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.fehbvm.com/Article/details/glrirxmod.sHtML

[S05] C：字符串长度
来源：http://read.share.zdbjq.cn/Article/details/gasbtytqa.sHtML

strlen(s)
来源：http://www.m.share.fehbvm.com/Article/details/gpjvubsta.sHtML

[S06] C：字符串比较
来源：http://3g.fehbvm.com/Article/details/gpiyexfqo.sHtML

strcmp(a, b) == 0
来源：http://3g.zdbjq.cn/Article/details/grbdhwqeg.sHtML

[S07] C：数组遍历求和
来源：http://mobile.fehbvm.com/Article/details/gtuphszzy.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.fehbvm.com/Article/details/gwrfuhsmw.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.hesvh.cn/Article/details/ghaljzpgr.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.zdbjq.cn/Article/details/gijkswlod.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.fehbvm.com/Article/details/gtdojtece.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.zdbjq.cn/Article/details/gkdhlbqtt.sHtML

[S10] C：指针与解引用
来源：http://baike.zdbjq.cn/Article/details/gphzvljld.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.fehbvm.com/Article/details/guvbedqxe.sHtML

[S11] C：逐行读文件
来源：http://mobile.fehbvm.com/Article/details/ghcoveqxl.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.fehbvm.com/Article/details/gpzrrjpps.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.fehbvm.com/Article/details/grbqmirgx.sHtML

fclose(f);
来源：http://3g.zdbjq.cn/Article/details/guafptllh.sHtML

[S12] C：写文件
来源：http://3g.zdbjq.cn/Article/details/goldfaznw.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.hesvh.cn/Article/details/gmgnwrken.sHtML

[S13] C：宏定义
来源：http://www.blog.zdbjq.cn/Article/details/geyeubzbt.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.fehbvm.com/Article/details/gcoxnuxvi.sHtML

[S14] C：枚举
来源：http://3g.fehbvm.com/Article/details/gjdarxoki.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.zdbjq.cn/Article/details/gbxvucgvs.sHtML

[S15] C：类型转换
来源：http://read.share.zdbjq.cn/Article/details/gkbeyzgbe.sHtML

(double) a / b
来源：http://m.share.zdbjq.cn/Article/details/gdblkjxyw.sHtML

[S16] C：位操作置位
来源：http://wap.zdbjq.cn/Article/details/glhihmzjg.sHtML

x |= (1 << 3);
来源：http://3g.fehbvm.com/Article/details/ginpqluvc.sHtML

[S17] C：安全拼接字符串
来源：http://blog.hesvh.cn/Article/details/gyfmqrcpj.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.hesvh.cn/Article/details/gsfwqsech.sHtML

[S18] C：命令行参数
来源：http://m.share.zdbjq.cn/Article/details/grwdgwvdw.sHtML

int main(int argc, char **argv)
来源：http://wap.hesvh.cn/Article/details/gxeqinfxa.sHtML

[S19] C：快速排序
来源：http://mobile.zdbjq.cn/Article/details/gafyyscxs.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.fehbvm.com/Article/details/gsloodxga.sHtML

[S20] C：二分查找
来源：http://baike.fehbvm.com/Article/details/gvgdtfoun.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.zdbjq.cn/Article/details/gwpvozeid.sHtML

[S21] C：字符类别判断
来源：http://3g.fehbvm.com/Article/details/gbstssszz.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.zdbjq.cn/Article/details/glatsmhgv.sHtML

[S22] C：字符串转数字
来源：http://3g.hesvh.cn/Article/details/gtqqsegkw.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.hesvh.cn/Article/details/gdhpbynut.sHtML

[S23] C：随机数
来源：http://www.blog.hesvh.cn/Article/details/gumjffljl.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.fehbvm.com/Article/details/gxibhfznd.sHtML

[S24] C：获取本地时间
来源：http://mobile.fehbvm.com/Article/details/goeqsjwvl.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.hesvh.cn/Article/details/ghgpawwxm.sHtML

[S25] C：内存拷贝
来源：http://www.share.fehbvm.com/Article/details/gxpqrrcqc.sHtML

memcpy(dst, src, n);
来源：http://www.share.fehbvm.com/Article/details/gzrjzmoxg.sHtML

[S26] C：内存清零
来源：http://wap.hesvh.cn/Article/details/gtiluiycz.sHtML

memset(a, 0, sizeof a);
来源：http://baike.zdbjq.cn/Article/details/gxicdrvsj.sHtML

[S27] C：定义常量
来源：http://mobile.fehbvm.com/Article/details/givwawsak.sHtML

const double PI = 3.14159;
来源：http://www.share.zdbjq.cn/Article/details/gribjlabs.sHtML

[S28] C：静态变量
来源：http://read.share.hesvh.cn/Article/details/gidjkibii.sHtML

static int counter = 0;
来源：http://read.share.fehbvm.com/Article/details/gxmkgnltx.sHtML

[S29] C：变参函数
来源：http://mobile.zdbjq.cn/Article/details/gtczqwblj.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.hesvh.cn/Article/details/grmxaohom.sHtML

[S30] C：头文件保护
来源：http://www.share.hesvh.cn/Article/details/ghclxsqhf.sHtML

#ifndef X_H
来源：http://read.share.hesvh.cn/Article/details/glxgllgav.sHtML

#define X_H
来源：http://www.blog.zdbjq.cn/Article/details/gdfhfarvy.sHtML

#endif
来源：http://baike.zdbjq.cn/Article/details/gnpimzyso.sHtML

[S31] C++：Hello World
来源：http://www.share.fehbvm.com/Article/details/gyjjdeomo.sHtML

#include <iostream>
来源：http://m.share.hesvh.cn/Article/details/gqnfvhhex.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.zdbjq.cn/Article/details/gyeoclhys.sHtML

[S32] C++：字符串
来源：http://read.share.zdbjq.cn/Article/details/gltzxnsaw.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.hesvh.cn/Article/details/gibalzrgc.sHtML

[S33] C++：vector 增删
来源：http://www.share.fehbvm.com/Article/details/gpzugnyxg.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.hesvh.cn/Article/details/gbtzafqpo.sHtML

[S34] C++：遍历 vector
来源：http://www.share.fehbvm.com/Article/details/gergabqbn.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.hesvh.cn/Article/details/gjptzbnvr.sHtML

[S35] C++：map
来源：http://www.share.zdbjq.cn/Article/details/glxvrhggx.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.fehbvm.com/Article/details/grzmzruxk.sHtML

[S36] C++：unordered_map
来源：http://m.share.zdbjq.cn/Article/details/gttvixzuh.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/ghzqwykjb.sHtML

[S37] C++：set
来源：http://www.share.hesvh.cn/Article/details/gkmyjgibt.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.fehbvm.com/Article/details/gyeozdnqe.sHtML

[S38] C++：排序
来源：http://baike.hesvh.cn/Article/details/ghllybeby.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.zdbjq.cn/Article/details/gtuvljypy.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.hesvh.cn/Article/details/gpqjjffvc.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.fehbvm.com/Article/details/gngcftdsx.sHtML

[S40] C++：查找元素
来源：http://www.blog.hesvh.cn/Article/details/gwuptmfkf.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.hesvh.cn/Article/details/gfmosxhxo.sHtML

[S41] C++：类与构造函数
来源：http://read.share.zdbjq.cn/Article/details/gncjekcks.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.zdbjq.cn/Article/details/girrmrwex.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.zdbjq.cn/Article/details/grzhxxfjw.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.hesvh.cn/Article/details/ggxxfxrdy.sHtML

[S43] C++：智能指针
来源：http://www.blog.hesvh.cn/Article/details/gjynfgmad.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.zdbjq.cn/Article/details/gmfjbfjgi.sHtML

[S44] C++：引用传参
来源：http://baike.fehbvm.com/Article/details/gahnlihwg.sHtML

void inc(int &x) { ++x; }
来源：http://3g.zdbjq.cn/Article/details/gpaiinkgi.sHtML

[S45] C++：lambda
来源：http://wap.zdbjq.cn/Article/details/ghvnwnnra.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.fehbvm.com/Article/details/ghvnorucv.sHtML

[S46] C++：函数模板
来源：http://www.m.share.fehbvm.com/Article/details/gyvtefabv.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.hesvh.cn/Article/details/grrfyfwvp.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.zdbjq.cn/Article/details/gerwlehpa.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.zdbjq.cn/Article/details/gpxpgjooc.sHtML

[S48] C++：逐行读文件
来源：http://blog.zdbjq.cn/Article/details/gffwkhncu.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.fehbvm.com/Article/details/gwcooipyj.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.hesvh.cn/Article/details/gonjwssft.sHtML

[S49] C++：写文件
来源：http://mobile.fehbvm.com/Article/details/gnhqavsqr.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.hesvh.cn/Article/details/geviyrobx.sHtML

[S50] C++：格式化数字
来源：http://wap.zdbjq.cn/Article/details/gmgzkewri.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.hesvh.cn/Article/details/gccvzmofk.sHtML

[S51] C++：显式类型转换
来源：http://m.share.hesvh.cn/Article/details/gjmuracgm.sHtML

static_cast<double>(a) / b
来源：http://3g.fehbvm.com/Article/details/gaywzaxly.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.fehbvm.com/Article/details/gdlqxinri.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.fehbvm.com/Article/details/gomyexgqz.sHtML

[S53] C++：移动语义
来源：http://www.m.share.fehbvm.com/Article/details/gocmpfzya.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.fehbvm.com/Article/details/gjonhubcr.sHtML

[S54] C++：异常处理
来源：http://blog.zdbjq.cn/Article/details/gsdblevgd.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.zdbjq.cn/Article/details/grmnnpvqg.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.hesvh.cn/Article/details/gcsvzqyti.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.hesvh.cn/Article/details/gzdarkwbv.sHtML

[S56] C++：optional
来源：http://mobile.fehbvm.com/Article/details/gufqgcrts.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.zdbjq.cn/Article/details/gpcpyxbca.sHtML

[S57] C++：编译期常量
来源：http://wap.zdbjq.cn/Article/details/gaxxfrdhn.sHtML

constexpr int N = 10;
来源：http://mobile.zdbjq.cn/Article/details/gpsttptcy.sHtML

[S58] C++：命名空间
来源：http://www.blog.hesvh.cn/Article/details/gvcvzdomp.sHtML

namespace ns { int f() { return 1; } }
来源：http://read.share.zdbjq.cn/Article/details/gxvwiafly.sHtML

[S59] C++：静态断言
来源：http://mobile.fehbvm.com/Article/details/gbikzoanu.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.fehbvm.com/Article/details/govlxyitw.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.zdbjq.cn/Article/details/gtueqyanz.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.zdbjq.cn/Article/details/gbnpkgfwd.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gladpdhob.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.zdbjq.cn/Article/details/geqdyhvxt.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gszfiwnbt.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.zdbjq.cn/Article/details/guzpoprjc.sHtML

println("Hello")
来源：http://blog.fehbvm.com/Article/details/gbkfqnojr.sHtML

[T02] Kotlin：变量
来源：http://www.blog.zdbjq.cn/Article/details/galymmdzs.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.zdbjq.cn/Article/details/gxqftvdvc.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.fehbvm.com/Article/details/gskzkdxet.sHtML

"值: $b"
来源：http://baike.fehbvm.com/Article/details/gtssqixsa.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.fehbvm.com/Article/details/ggcchvozc.sHtML

val n: String? = null;  n?.length
来源：http://baike.hesvh.cn/Article/details/gpnjlviht.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.fehbvm.com/Article/details/gfpxlsfee.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.hesvh.cn/Article/details/goiebtbgh.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.hesvh.cn/Article/details/glnqebjff.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://mobile.hesvh.cn/Article/details/gmrlldpqp.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.zdbjq.cn/Article/details/gwcrdxwvs.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://baike.hesvh.cn/Article/details/gdbgkymsu.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.fehbvm.com/Article/details/gfhoinrhp.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.hesvh.cn/Article/details/gchadrcxt.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.fehbvm.com/Article/details/ghakcfjsc.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.hesvh.cn/Article/details/gtjtiddbk.sHtML

[T10] Kotlin：默认参数
来源：http://baike.fehbvm.com/Article/details/gxwruwxwv.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.hesvh.cn/Article/details/grvxwxkvm.sHtML

[T11] Kotlin：协程
来源：http://mobile.zdbjq.cn/Article/details/gutwbxogw.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://read.share.fehbvm.com/Article/details/guwayrbyp.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.hesvh.cn/Article/details/guaudcevg.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.fehbvm.com/Article/details/ggoklywri.sHtML

[T13] Kotlin：只读 Map
来源：http://www.blog.fehbvm.com/Article/details/gxesvippx.sHtML

val m = mapOf("a" to 1)
来源：http://www.share.zdbjq.cn/Article/details/gvewdiwan.sHtML

[T14] Kotlin：循环
来源：http://3g.fehbvm.com/Article/details/gulaqontn.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.fehbvm.com/Article/details/gvvcgjmbt.sHtML

[T15] Kotlin：接口
来源：http://3g.fehbvm.com/Article/details/gjkecmxzu.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.fehbvm.com/Article/details/ghkcnrucg.sHtML

[T16] Swift：Hello World
来源：http://mobile.fehbvm.com/Article/details/guecubygd.sHtML

print("Hello")
来源：http://mobile.fehbvm.com/Article/details/gqoavnzxv.sHtML

[T17] Swift：变量与常量
来源：http://www.share.fehbvm.com/Article/details/gsphraxhf.sHtML

var a = 1;  let b = 2
来源：http://www.share.zdbjq.cn/Article/details/gbcssisuf.sHtML

[T18] Swift：字符串插值
来源：http://wap.hesvh.cn/Article/details/gafcpwivk.sHtML

"值: \(b)"
来源：http://3g.hesvh.cn/Article/details/gwrehyokx.sHtML

[T19] Swift：可选绑定
来源：http://www.m.share.hesvh.cn/Article/details/gpzwdvqar.sHtML

if let n = opt { print(n) }
来源：http://baike.zdbjq.cn/Article/details/gengluelg.sHtML

[T20] Swift：数组操作
来源：http://www.m.share.fehbvm.com/Article/details/gyoktqhqz.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://wap.fehbvm.com/Article/details/gucqcbeoh.sHtML

[T21] Swift：遍历
来源：http://wap.fehbvm.com/Article/details/gwzucvsjb.sHtML

for x in a { print(x) }
来源：http://www.m.share.hesvh.cn/Article/details/gqmiuhxtd.sHtML

[T22] Swift：字典
来源：http://3g.hesvh.cn/Article/details/guxgtwnrt.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://m.share.hesvh.cn/Article/details/gwzcpvjrz.sHtML

[T23] Swift：函数
来源：http://wap.hesvh.cn/Article/details/gxswjtawc.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wap.zdbjq.cn/Article/details/gretytzul.sHtML

[T24] Swift：闭包
来源：http://www.m.share.hesvh.cn/Article/details/ggcjquupd.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://blog.hesvh.cn/Article/details/ghlitwxtr.sHtML

[T25] Swift：结构体
来源：http://baike.fehbvm.com/Article/details/gvikxyfyi.sHtML

struct P { var x: Int }
来源：http://www.blog.fehbvm.com/Article/details/gkyxyhhrz.sHtML

[T26] Swift：类与重写
来源：http://blog.fehbvm.com/Article/details/gdqsggrdw.sHtML

class A: Base { override func f() {} }
来源：http://m.share.zdbjq.cn/Article/details/gshccsvxm.sHtML

[T27] Swift：错误处理
来源：http://www.share.zdbjq.cn/Article/details/gqwwguinr.sHtML

do { try f() } catch { print(error) }
来源：http://mobile.hesvh.cn/Article/details/gogohyrpa.sHtML

[T28] Swift：枚举
来源：http://www.share.hesvh.cn/Article/details/gizsytlao.sHtML

enum Color { case red, green }
来源：http://wap.zdbjq.cn/Article/details/gbdxgaoje.sHtML

[T29] Swift：guard 提前返回
来源：http://wap.hesvh.cn/Article/details/gupeiiesf.sHtML

guard let x = opt else { return }
来源：http://wap.fehbvm.com/Article/details/gicbtcirb.sHtML

[T30] Swift：协议
来源：http://m.share.fehbvm.com/Article/details/gicufdtvc.sHtML

protocol Shape { func area() -> Double }
来源：http://wap.fehbvm.com/Article/details/gsefggzos.sHtML

[T31] Lua：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gbgmrplbl.sHtML

print("Hello")
来源：http://blog.fehbvm.com/Article/details/gzpyqpzlr.sHtML

[T32] Lua：局部变量
来源：http://read.share.hesvh.cn/Article/details/gnpaowxid.sHtML

local a = 1
来源：http://baike.zdbjq.cn/Article/details/gvoiyenqa.sHtML


<!-- 参考信息 -->