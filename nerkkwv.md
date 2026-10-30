代发 wailian999

f() { local x=1; echo "$x"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggnfynwfe.sHtML

[R32] 参数个数校验
来源：http://m.share.fanxiaobao.xyz/Article/details/gipidgxda.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gbsxkbxgi.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvbhxslvo.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.fanxiaobao.xyz/Article/details/gbyvextlh.sHtML

[R34] 退出时清理
来源：http://3g.fanxiaobao.xyz/Article/details/gsgditwne.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gukqnzlki.sHtML

[R35] 后台执行并等待
来源：http://wap.fanxiaobao.xyz/Article/details/gyvoljejk.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geeqrounu.sHtML

[R36] 并发执行多个任务
来源：http://read.share.fanxiaobao.xyz/Article/details/grsrpbxwe.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvaolbnvn.sHtML

[R37] 把输出赋给变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gkbmekmyi.sHtML

files=$(ls -1)
来源：http://mobile.fanxiaobao.xyz/Article/details/gymtrxndr.sHtML

[R38] 管道串联
来源：http://m.share.fanxiaobao.xyz/Article/details/ggybtygpg.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.fanxiaobao.xyz/Article/details/ghhbhvosv.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.fanxiaobao.xyz/Article/details/gqstlwpyd.sHtML

cmd > out.log 2>&1
来源：http://mobile.fanxiaobao.xyz/Article/details/gmnsaausq.sHtML

[R40] 追加写日志
来源：http://blog.fanxiaobao.xyz/Article/details/gqfrkqtkp.sHtML

echo "log" >> out.log
来源：http://www.blog.fanxiaobao.xyz/Article/details/gygweybvu.sHtML

[R41] 丢弃输出
来源：http://blog.fanxiaobao.xyz/Article/details/gsqxygvxa.sHtML

cmd >/dev/null 2>&1
来源：http://baike.fanxiaobao.xyz/Article/details/gjlsoawqq.sHtML

[R42] 输入重定向
来源：http://baike.fanxiaobao.xyz/Article/details/guyungvxh.sHtML

wc -l < a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gkwhjwkvi.sHtML

[R43] 按名字查找文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gxhuysxmu.sHtML

find . -name "*.log" -type f
来源：http://read.share.fanxiaobao.xyz/Article/details/grtrggscl.sHtML

[R44] 按修改时间查找
来源：http://baike.fanxiaobao.xyz/Article/details/gowyjewpn.sHtML

find . -mtime -7 -type f
来源：http://blog.fanxiaobao.xyz/Article/details/gkxbrnsyn.sHtML

[R45] 批量删除
来源：http://wap.fanxiaobao.xyz/Article/details/grnqsukai.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gemxzddlt.sHtML

[R46] 递归替换文件内容
来源：http://read.share.fanxiaobao.xyz/Article/details/gfyyojryv.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.fanxiaobao.xyz/Article/details/gsqplupuj.sHtML

[R47] sed 单行替换
来源：http://wap.fanxiaobao.xyz/Article/details/gyobgmhdv.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/grdejxibu.sHtML

[R48] awk 取指定列
来源：http://3g.fanxiaobao.xyz/Article/details/gvjbskncu.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghjrtqzrc.sHtML

[R49] awk 带条件
来源：http://read.share.fanxiaobao.xyz/Article/details/gohmlbquc.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkadvauch.sHtML

[R50] awk 求和
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geqdtjqbz.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gaxgnqclz.sHtML

[R51] 排序去重取前几
来源：http://baike.fanxiaobao.xyz/Article/details/gcrfqnpfx.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.fanxiaobao.xyz/Article/details/guorvzune.sHtML

[R52] 统计行数
来源：http://mobile.fanxiaobao.xyz/Article/details/gxfypmcqv.sHtML

wc -l a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/grqeduubt.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.fanxiaobao.xyz/Article/details/gtnbaihhl.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.fanxiaobao.xyz/Article/details/gxvcyrfki.sHtML

[R54] 比较两个文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gamktkmks.sHtML

diff a.txt b.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gsmpuwjqd.sHtML

[R55] 压缩与解压
来源：http://blog.fanxiaobao.xyz/Article/details/gmxvgcpry.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://baike.fanxiaobao.xyz/Article/details/gxpnnjmdb.sHtML

[R56] 远程拷贝
来源：http://3g.fanxiaobao.xyz/Article/details/gahkrxgej.sHtML

scp file user@host:/path/
来源：http://wap.fanxiaobao.xyz/Article/details/ghhitkwtj.sHtML

[R57] 远程执行命令
来源：http://www.share.fanxiaobao.xyz/Article/details/gwvromiww.sHtML

ssh user@host 'uptime'
来源：http://m.share.fanxiaobao.xyz/Article/details/gagzuilzq.sHtML

[R58] 下载文件
来源：http://wap.fanxiaobao.xyz/Article/details/gkniajdtn.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.fanxiaobao.xyz/Article/details/gstptvnye.sHtML

[R59] 发 POST JSON
来源：http://blog.fanxiaobao.xyz/Article/details/gwfxlqlhz.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.fanxiaobao.xyz/Article/details/gvjdlbcpt.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggpymdcwo.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.fanxiaobao.xyz/Article/details/gcbxkhlhf.sHtML

[R61] 磁盘占用
来源：http://3g.fanxiaobao.xyz/Article/details/gpsibkqqr.sHtML

df -h;  du -sh *
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfyesrjmi.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpylqsort.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.fanxiaobao.xyz/Article/details/gwfywwurt.sHtML

[R63] 内存与进程
来源：http://blog.fanxiaobao.xyz/Article/details/ginvdpjkt.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.fanxiaobao.xyz/Article/details/gwjuuyfko.sHtML

[R64] 结束进程
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaqtzickh.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.fanxiaobao.xyz/Article/details/gpfiypvgu.sHtML

[R65] 查看端口占用
来源：http://www.share.fanxiaobao.xyz/Article/details/gxpgkrhnq.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.fanxiaobao.xyz/Article/details/gfqchrqbo.sHtML

[R66] 定时任务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjqzmyltl.sHtML

crontab -e;  crontab -l
来源：http://3g.fanxiaobao.xyz/Article/details/gddfqkdqe.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.fanxiaobao.xyz/Article/details/gguvxggnn.sHtML

openssl rand -hex 16
来源：http://3g.fanxiaobao.xyz/Article/details/gguaenbzt.sHtML

[R68] 计算文件校验值
来源：http://read.share.fanxiaobao.xyz/Article/details/gwohejyqb.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gecwdeltl.sHtML

[R69] 生成随机密码
来源：http://www.blog.fanxiaobao.xyz/Article/details/glowraylw.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.fanxiaobao.xyz/Article/details/gixecsgcq.sHtML

[R70] 时间戳与互转
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzhnwvgtz.sHtML

date +%s;  date -d @1700000000
来源：http://m.share.fanxiaobao.xyz/Article/details/gjzzooyrr.sHtML

[R71] 日期格式化
来源：http://mobile.fanxiaobao.xyz/Article/details/geooyrtfh.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.fanxiaobao.xyz/Article/details/gbgmegrnm.sHtML

[R72] 等待端口就绪
来源：http://read.share.fanxiaobao.xyz/Article/details/ghlgxtqfv.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gluxpfrmo.sHtML

[R73] 分割大日志
来源：http://baike.fanxiaobao.xyz/Article/details/gdgdvrnoo.sHtML

split -l 1000 big.log part_
来源：http://read.share.fanxiaobao.xyz/Article/details/gwjuodvmn.sHtML

[R74] 批量重命名
来源：http://blog.fanxiaobao.xyz/Article/details/gcluvqrqz.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/grfdtkqmq.sHtML

[R75] 导出环境变量
来源：http://blog.fanxiaobao.xyz/Article/details/gvqpavgdx.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.fanxiaobao.xyz/Article/details/gxgjktarq.sHtML

[R76] 使用临时文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gntmjfetk.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fanxiaobao.xyz/Article/details/gpyawxuer.sHtML

[R77] 读取用户输入
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyencglkn.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtuwhqxky.sHtML

[R78] 交互式菜单
来源：http://blog.fanxiaobao.xyz/Article/details/gqvuplgqz.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geewnrymf.sHtML

[R79] 解析命令行选项
来源：http://blog.fanxiaobao.xyz/Article/details/gfhrpjlbm.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gttpotnhd.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqfchtbmy.sHtML

time ./run.sh
来源：http://read.share.fanxiaobao.xyz/Article/details/gzdumikez.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gxdvubihg.sHtML

S. C / C++ 专题
来源：http://m.share.fanxiaobao.xyz/Article/details/grqeiixaa.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gwvcvtvmo.sHtML

[S01] C：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/ghyufunkr.sHtML

#include <stdio.h>
来源：http://blog.fanxiaobao.xyz/Article/details/gveejlnpd.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzlrwvmvi.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbseblvoi.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.fanxiaobao.xyz/Article/details/gasyhjjpz.sHtML

[S03] C：读入整数
来源：http://read.share.fanxiaobao.xyz/Article/details/gzvlkgrow.sHtML

int x; scanf("%d", &x);
来源：http://blog.fanxiaobao.xyz/Article/details/gtciyrahm.sHtML

[S04] C：字符串复制
来源：http://baike.fanxiaobao.xyz/Article/details/gqvzcxmig.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.fanxiaobao.xyz/Article/details/ghrttqybt.sHtML

[S05] C：字符串长度
来源：http://blog.fanxiaobao.xyz/Article/details/gstkunckk.sHtML

strlen(s)
来源：http://www.share.fanxiaobao.xyz/Article/details/gxdisgolj.sHtML

[S06] C：字符串比较
来源：http://m.share.fanxiaobao.xyz/Article/details/gxhdafdke.sHtML

strcmp(a, b) == 0
来源：http://read.share.fanxiaobao.xyz/Article/details/glticxios.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gggsvkjna.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpiwylvyu.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.fanxiaobao.xyz/Article/details/gxxovofsh.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.fanxiaobao.xyz/Article/details/gtrrgnqih.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkovtpvzl.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.fanxiaobao.xyz/Article/details/gstsjuqkt.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guslhahck.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.fanxiaobao.xyz/Article/details/gouevzept.sHtML

[S11] C：逐行读文件
来源：http://baike.fanxiaobao.xyz/Article/details/gexqvjprl.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.fanxiaobao.xyz/Article/details/gggnsnxpu.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.fanxiaobao.xyz/Article/details/gmrqewvvs.sHtML

fclose(f);
来源：http://mobile.fanxiaobao.xyz/Article/details/gmnuawvvb.sHtML

[S12] C：写文件
来源：http://wap.fanxiaobao.xyz/Article/details/gunxonjpv.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbtrmjknp.sHtML

[S13] C：宏定义
来源：http://read.share.fanxiaobao.xyz/Article/details/gckafdpyq.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.fanxiaobao.xyz/Article/details/gylpxpzed.sHtML

[S14] C：枚举
来源：http://www.blog.fanxiaobao.xyz/Article/details/gexfxssum.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.fanxiaobao.xyz/Article/details/gcchnrclz.sHtML

[S15] C：类型转换
来源：http://3g.fanxiaobao.xyz/Article/details/ggszfcgtq.sHtML

(double) a / b
来源：http://m.share.fanxiaobao.xyz/Article/details/gabevrxcg.sHtML

[S16] C：位操作置位
来源：http://wap.fanxiaobao.xyz/Article/details/gybejdcfo.sHtML

x |= (1 << 3);
来源：http://3g.fanxiaobao.xyz/Article/details/gmgpkbwtl.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtlpgqewt.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.fanxiaobao.xyz/Article/details/gweprsytj.sHtML

[S18] C：命令行参数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gscclfxwr.sHtML

int main(int argc, char **argv)
来源：http://wap.fanxiaobao.xyz/Article/details/ggeprlmrq.sHtML

[S19] C：快速排序
来源：http://mobile.fanxiaobao.xyz/Article/details/gnzyazliv.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.fanxiaobao.xyz/Article/details/gwecubygp.sHtML

[S20] C：二分查找
来源：http://3g.fanxiaobao.xyz/Article/details/gbmbbqlrw.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.fanxiaobao.xyz/Article/details/guihzxlpd.sHtML

[S21] C：字符类别判断
来源：http://www.share.fanxiaobao.xyz/Article/details/gyvgdeskj.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.fanxiaobao.xyz/Article/details/gzegoqrjs.sHtML

[S22] C：字符串转数字
来源：http://3g.fanxiaobao.xyz/Article/details/guihfjjzx.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gigylgjtd.sHtML

[S23] C：随机数
来源：http://m.share.fanxiaobao.xyz/Article/details/gtpdyzmoh.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.fanxiaobao.xyz/Article/details/gcbgzrzih.sHtML

[S24] C：获取本地时间
来源：http://3g.fanxiaobao.xyz/Article/details/gkligsmnk.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.fanxiaobao.xyz/Article/details/gozsvudlj.sHtML

[S25] C：内存拷贝
来源：http://wap.fanxiaobao.xyz/Article/details/geoyfhwuv.sHtML

memcpy(dst, src, n);
来源：http://wap.fanxiaobao.xyz/Article/details/gcxhbascp.sHtML

[S26] C：内存清零
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmcmgwlax.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.fanxiaobao.xyz/Article/details/gvzsbpbop.sHtML

[S27] C：定义常量
来源：http://read.share.fanxiaobao.xyz/Article/details/ghbdnhawt.sHtML

const double PI = 3.14159;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmgvebszs.sHtML

[S28] C：静态变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gnloexmif.sHtML

static int counter = 0;
来源：http://baike.fanxiaobao.xyz/Article/details/guvmkqgkx.sHtML

[S29] C：变参函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gnajbumlx.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.fanxiaobao.xyz/Article/details/gawlgyvbh.sHtML

[S30] C：头文件保护
来源：http://blog.fanxiaobao.xyz/Article/details/gecxskpwz.sHtML

#ifndef X_H
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmvkiodmi.sHtML

#define X_H
来源：http://m.share.fanxiaobao.xyz/Article/details/gzblsghqb.sHtML

#endif
来源：http://read.share.fanxiaobao.xyz/Article/details/gkjoyzllt.sHtML

[S31] C++：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcrwnrzrd.sHtML

#include <iostream>
来源：http://www.share.fanxiaobao.xyz/Article/details/ggscpudjp.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gihwkvucx.sHtML

[S32] C++：字符串
来源：http://baike.fanxiaobao.xyz/Article/details/gfnmagxgv.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.fanxiaobao.xyz/Article/details/gktxyjtqy.sHtML

[S33] C++：vector 增删
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfxyqjtpo.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.fanxiaobao.xyz/Article/details/gwsnvnwup.sHtML

[S34] C++：遍历 vector
来源：http://wap.fanxiaobao.xyz/Article/details/guxwrrdps.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gamastyuk.sHtML

[S35] C++：map
来源：http://3g.fanxiaobao.xyz/Article/details/gjpwsflpc.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/goukrrkxa.sHtML

[S36] C++：unordered_map
来源：http://wap.fanxiaobao.xyz/Article/details/gjgrjzpbr.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gjzvzuerh.sHtML

[S37] C++：set
来源：http://baike.fanxiaobao.xyz/Article/details/gxdvpfagw.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.fanxiaobao.xyz/Article/details/gnnjkzstg.sHtML

[S38] C++：排序
来源：http://m.share.fanxiaobao.xyz/Article/details/geyuzxzvf.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvkztwxct.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.fanxiaobao.xyz/Article/details/gkiwupqee.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.fanxiaobao.xyz/Article/details/grvpjusgh.sHtML

[S40] C++：查找元素
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkzdaosat.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.fanxiaobao.xyz/Article/details/gzrfsnbct.sHtML

[S41] C++：类与构造函数
来源：http://3g.fanxiaobao.xyz/Article/details/gwjoipsti.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.fanxiaobao.xyz/Article/details/gliqbvitt.sHtML

[S42] C++：继承与虚函数
来源：http://blog.fanxiaobao.xyz/Article/details/gpplgkrex.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.fanxiaobao.xyz/Article/details/glzostqdm.sHtML

[S43] C++：智能指针
来源：http://www.share.fanxiaobao.xyz/Article/details/gnzqqrtfh.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.fanxiaobao.xyz/Article/details/grmqfytof.sHtML

[S44] C++：引用传参
来源：http://m.share.fanxiaobao.xyz/Article/details/gtohmuxzv.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.fanxiaobao.xyz/Article/details/guauwqpbo.sHtML

[S45] C++：lambda
来源：http://blog.fanxiaobao.xyz/Article/details/gtqcjfpix.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.fanxiaobao.xyz/Article/details/ggpdfbzmc.sHtML

[S46] C++：函数模板
来源：http://m.share.fanxiaobao.xyz/Article/details/gifbmpgjc.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.fanxiaobao.xyz/Article/details/guiwkgmop.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.fanxiaobao.xyz/Article/details/gpkbvggyf.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfdbsuxws.sHtML

[S48] C++：逐行读文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gmxmhnmfw.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.fanxiaobao.xyz/Article/details/gewfgtaar.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjsrgujjk.sHtML

[S49] C++：写文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gnitjptsb.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.fanxiaobao.xyz/Article/details/gyljsovyn.sHtML

[S50] C++：格式化数字
来源：http://m.share.fanxiaobao.xyz/Article/details/gshbuagfx.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.fanxiaobao.xyz/Article/details/gehykqqdy.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glewerfzb.sHtML

static_cast<double>(a) / b
来源：http://mobile.fanxiaobao.xyz/Article/details/grfcaihuo.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.fanxiaobao.xyz/Article/details/gdimnfivb.sHtML

int size() const noexcept { return n_; }
来源：http://blog.fanxiaobao.xyz/Article/details/gyrwddjub.sHtML

[S53] C++：移动语义
来源：http://3g.fanxiaobao.xyz/Article/details/gvumqddwx.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.fanxiaobao.xyz/Article/details/gllyxrhjx.sHtML

[S54] C++：异常处理
来源：http://m.share.fanxiaobao.xyz/Article/details/gyrrtniuw.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.fanxiaobao.xyz/Article/details/gvwkjmmeh.sHtML

[S55] C++：结构化绑定
来源：http://read.share.fanxiaobao.xyz/Article/details/gdniwwluc.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gasxsnefd.sHtML

[S56] C++：optional
来源：http://mobile.fanxiaobao.xyz/Article/details/gxgadkkxd.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.fanxiaobao.xyz/Article/details/gkgoyklfg.sHtML

[S57] C++：编译期常量
来源：http://read.share.fanxiaobao.xyz/Article/details/gcjjxxiwo.sHtML

constexpr int N = 10;
来源：http://mobile.fanxiaobao.xyz/Article/details/gzutkskxb.sHtML

[S58] C++：命名空间
来源：http://wap.fanxiaobao.xyz/Article/details/ghsfenhre.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.fanxiaobao.xyz/Article/details/glmtcmahd.sHtML

[S59] C++：静态断言
来源：http://baike.fanxiaobao.xyz/Article/details/gyzqfnctm.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.fanxiaobao.xyz/Article/details/gxmspemjc.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.fanxiaobao.xyz/Article/details/ghuipsbbd.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.fanxiaobao.xyz/Article/details/gmqmlrjep.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gclhnjedy.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.fanxiaobao.xyz/Article/details/guhkapyjj.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/ghvsfcbrs.sHtML

[T01] Kotlin：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyemcbczh.sHtML

println("Hello")
来源：http://m.share.fanxiaobao.xyz/Article/details/gmlufmeuo.sHtML

[T02] Kotlin：变量
来源：http://3g.fanxiaobao.xyz/Article/details/gwqkszthv.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.fanxiaobao.xyz/Article/details/gslukdgsv.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.fanxiaobao.xyz/Article/details/gwrxlbhby.sHtML

"值: $b"
来源：http://m.share.fanxiaobao.xyz/Article/details/giycyflco.sHtML

[T04] Kotlin：空安全
来源：http://m.share.fanxiaobao.xyz/Article/details/glbhpvald.sHtML

val n: String? = null;  n?.length
来源：http://baike.fanxiaobao.xyz/Article/details/grfozmnnt.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.fanxiaobao.xyz/Article/details/gsmydjlvr.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.fanxiaobao.xyz/Article/details/gqjtozcbr.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.fanxiaobao.xyz/Article/details/gpunksmlk.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.fanxiaobao.xyz/Article/details/gzshebqxu.sHtML

[T07] Kotlin：集合过滤
来源：http://blog.fanxiaobao.xyz/Article/details/gzibvnpen.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gziweyjym.sHtML

[T08] Kotlin：数据类
来源：http://read.share.fanxiaobao.xyz/Article/details/guimzdely.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.fanxiaobao.xyz/Article/details/ggsphldhs.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gbiqphboe.sHtML

fun String.exclaim() = this + "!"
来源：http://wap.fanxiaobao.xyz/Article/details/gifptxwzh.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.fanxiaobao.xyz/Article/details/gztomnfue.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.fanxiaobao.xyz/Article/details/gmnppyogh.sHtML

[T11] Kotlin：协程
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzfmsvwsl.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkkxdlkxb.sHtML

[T12] Kotlin：解构声明
来源：http://www.share.fanxiaobao.xyz/Article/details/gkfnarbui.sHtML

val (a, b) = Pair(1, 2)
来源：http://mobile.fanxiaobao.xyz/Article/details/ghjpsbguv.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghfjjulma.sHtML

val m = mapOf("a" to 1)
来源：http://wap.fanxiaobao.xyz/Article/details/gqqfedzfz.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gopbxeeie.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.fanxiaobao.xyz/Article/details/guqnooqry.sHtML

[T15] Kotlin：接口
来源：http://baike.fanxiaobao.xyz/Article/details/gccgckjoc.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.fanxiaobao.xyz/Article/details/glcyivxxc.sHtML

[T16] Swift：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gistxxvmc.sHtML

print("Hello")
来源：http://mobile.fanxiaobao.xyz/Article/details/gxbkqmzbk.sHtML

[T17] Swift：变量与常量
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggghklsqa.sHtML

var a = 1;  let b = 2
来源：http://www.share.fanxiaobao.xyz/Article/details/gtnjxwdwx.sHtML

[T18] Swift：字符串插值
来源：http://mobile.fanxiaobao.xyz/Article/details/gvdfpyvyz.sHtML

"值: \(b)"
来源：http://read.share.fanxiaobao.xyz/Article/details/gxfksrysf.sHtML

[T19] Swift：可选绑定
来源：http://blog.fanxiaobao.xyz/Article/details/ggonbjdlu.sHtML

if let n = opt { print(n) }
来源：http://blog.fanxiaobao.xyz/Article/details/gxcnndcbn.sHtML

[T20] Swift：数组操作
来源：http://read.share.fanxiaobao.xyz/Article/details/gvykpwcdu.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://wap.fanxiaobao.xyz/Article/details/gcaeyfhcw.sHtML

[T21] Swift：遍历
来源：http://blog.fanxiaobao.xyz/Article/details/gxndxdwxn.sHtML

for x in a { print(x) }
来源：http://www.share.fanxiaobao.xyz/Article/details/grdgnkigk.sHtML

[T22] Swift：字典
来源：http://baike.fanxiaobao.xyz/Article/details/ghwvjbspk.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://baike.fanxiaobao.xyz/Article/details/gygsfdhib.sHtML

[T23] Swift：函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gzvebdmvr.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://read.share.fanxiaobao.xyz/Article/details/gesfdtizc.sHtML

[T24] Swift：闭包
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gecwysnne.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://blog.fanxiaobao.xyz/Article/details/gsmghtose.sHtML

[T25] Swift：结构体
来源：http://read.share.fanxiaobao.xyz/Article/details/gglslthpi.sHtML

struct P { var x: Int }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjnrbzxkz.sHtML

[T26] Swift：类与重写
来源：http://m.share.fanxiaobao.xyz/Article/details/gxzgjlubz.sHtML

class A: Base { override func f() {} }
来源：http://m.share.fanxiaobao.xyz/Article/details/ghagjljwc.sHtML

[T27] Swift：错误处理
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqzeiygxo.sHtML

do { try f() } catch { print(error) }
来源：http://blog.fanxiaobao.xyz/Article/details/gldrlnssq.sHtML

[T28] Swift：枚举
来源：http://m.share.fanxiaobao.xyz/Article/details/gfpebrxzf.sHtML

enum Color { case red, green }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvagfudze.sHtML

[T29] Swift：guard 提前返回
来源：http://3g.fanxiaobao.xyz/Article/details/gmobotqam.sHtML

guard let x = opt else { return }
来源：http://wap.fanxiaobao.xyz/Article/details/gxlpvqgyz.sHtML

[T30] Swift：协议
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghgipfioo.sHtML

protocol Shape { func area() -> Double }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyldbkiwu.sHtML

[T31] Lua：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfbtaadwm.sHtML

print("Hello")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnkepkqwr.sHtML

[T32] Lua：局部变量
来源：http://baike.fanxiaobao.xyz/Article/details/gbklajszu.sHtML

local a = 1
来源：http://m.share.fanxiaobao.xyz/Article/details/gjkkvqocv.sHtML

[T33] Lua：表（数组）
来源：http://www.share.fanxiaobao.xyz/Article/details/gddfhcsiq.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://read.share.fanxiaobao.xyz/Article/details/gkoxnentz.sHtML

[T34] Lua：遍历表
来源：http://m.share.fanxiaobao.xyz/Article/details/gdbouayhj.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://blog.fanxiaobao.xyz/Article/details/gkoepfxst.sHtML


<!-- 参考信息 -->