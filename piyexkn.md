代发 wailian999

echo $((1 + 2 * 3))
来源：http://read.share.fanxiaobao.xyz/Article/details/gssycitus.sHtML

[R28] 浮点运算
来源：http://read.share.fanxiaobao.xyz/Article/details/gifdlmtnj.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.fanxiaobao.xyz/Article/details/gcbrxvksj.sHtML

[R29] 定义函数
来源：http://blog.fanxiaobao.xyz/Article/details/gspzefhwt.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.fanxiaobao.xyz/Article/details/gvaikcyxv.sHtML

[R30] 函数返回状态码
来源：http://blog.fanxiaobao.xyz/Article/details/gtplxmrij.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.fanxiaobao.xyz/Article/details/gqmnhhuvw.sHtML

[R31] 局部变量
来源：http://blog.fanxiaobao.xyz/Article/details/gtseqysci.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gizcoppgq.sHtML

[R32] 参数个数校验
来源：http://blog.fanxiaobao.xyz/Article/details/gkegyiosa.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gkhngmclz.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.fanxiaobao.xyz/Article/details/gemkjvdxn.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.fanxiaobao.xyz/Article/details/gybthkjxw.sHtML

[R34] 退出时清理
来源：http://mobile.fanxiaobao.xyz/Article/details/ghmfuwqvm.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.fanxiaobao.xyz/Article/details/gwnqrvsdd.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjphnndmb.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.fanxiaobao.xyz/Article/details/gbuequvam.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdujcjdru.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.fanxiaobao.xyz/Article/details/gtskadtaw.sHtML

[R37] 把输出赋给变量
来源：http://blog.fanxiaobao.xyz/Article/details/gnbivdood.sHtML

files=$(ls -1)
来源：http://read.share.fanxiaobao.xyz/Article/details/gwkprtbai.sHtML

[R38] 管道串联
来源：http://blog.fanxiaobao.xyz/Article/details/gihzhfvpk.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.fanxiaobao.xyz/Article/details/gyjglgmhw.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkviedwsr.sHtML

cmd > out.log 2>&1
来源：http://wap.fanxiaobao.xyz/Article/details/gcyrvnzby.sHtML

[R40] 追加写日志
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqmgjnmgv.sHtML

echo "log" >> out.log
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqbavulxp.sHtML

[R41] 丢弃输出
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbygyqfau.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.fanxiaobao.xyz/Article/details/gguihmair.sHtML

[R42] 输入重定向
来源：http://mobile.fanxiaobao.xyz/Article/details/gyhsxyoqg.sHtML

wc -l < a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gdijqbhvb.sHtML

[R43] 按名字查找文件
来源：http://read.share.fanxiaobao.xyz/Article/details/ghsbpjxgw.sHtML

find . -name "*.log" -type f
来源：http://www.blog.fanxiaobao.xyz/Article/details/grgmehsjc.sHtML

[R44] 按修改时间查找
来源：http://mobile.fanxiaobao.xyz/Article/details/gemvojurz.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grbqrxyun.sHtML

[R45] 批量删除
来源：http://blog.fanxiaobao.xyz/Article/details/gkfialyky.sHtML

find . -name "*.tmp" -delete
来源：http://blog.fanxiaobao.xyz/Article/details/guttgovyx.sHtML

[R46] 递归替换文件内容
来源：http://3g.fanxiaobao.xyz/Article/details/gyejecmxz.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.fanxiaobao.xyz/Article/details/gtpuzzbda.sHtML

[R47] sed 单行替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gknnvtayz.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gnzhqazji.sHtML

[R48] awk 取指定列
来源：http://www.share.fanxiaobao.xyz/Article/details/gwynflbct.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gaiybbnyu.sHtML

[R49] awk 带条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdvketveq.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.fanxiaobao.xyz/Article/details/gxadqmkas.sHtML

[R50] awk 求和
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsrbzjynr.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/grgpoupor.sHtML

[R51] 排序去重取前几
来源：http://www.share.fanxiaobao.xyz/Article/details/gzcvcadja.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbmegxeuf.sHtML

[R52] 统计行数
来源：http://wap.fanxiaobao.xyz/Article/details/gyrtlrxua.sHtML

wc -l a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/galjpmgnl.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.fanxiaobao.xyz/Article/details/gegngmxyv.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.fanxiaobao.xyz/Article/details/gdjnnudnt.sHtML

[R54] 比较两个文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gryuxvpui.sHtML

diff a.txt b.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gdugavmkt.sHtML

[R55] 压缩与解压
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsxffqkgq.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.fanxiaobao.xyz/Article/details/gfzngtbwa.sHtML

[R56] 远程拷贝
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjnrtafkr.sHtML

scp file user@host:/path/
来源：http://baike.fanxiaobao.xyz/Article/details/gekuqxxzg.sHtML

[R57] 远程执行命令
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnjcxtykj.sHtML

ssh user@host 'uptime'
来源：http://www.share.fanxiaobao.xyz/Article/details/govnjruap.sHtML

[R58] 下载文件
来源：http://baike.fanxiaobao.xyz/Article/details/ggrozrups.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.fanxiaobao.xyz/Article/details/gittgylfj.sHtML

[R59] 发 POST JSON
来源：http://blog.fanxiaobao.xyz/Article/details/gvwnofddj.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.fanxiaobao.xyz/Article/details/gjnwjxhbv.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.fanxiaobao.xyz/Article/details/gauhupycy.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.fanxiaobao.xyz/Article/details/gimtosmvn.sHtML

[R61] 磁盘占用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkeyeawyb.sHtML

df -h;  du -sh *
来源：http://read.share.fanxiaobao.xyz/Article/details/gqvzmqpov.sHtML

[R62] 找最占空间的文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gqbnhtrnj.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.fanxiaobao.xyz/Article/details/gvczlhdqt.sHtML

[R63] 内存与进程
来源：http://wap.fanxiaobao.xyz/Article/details/gmgvywims.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grdyysbqf.sHtML

[R64] 结束进程
来源：http://www.blog.fanxiaobao.xyz/Article/details/gudmfcrkj.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gidhowsbe.sHtML

[R65] 查看端口占用
来源：http://3g.fanxiaobao.xyz/Article/details/gdnaidwuh.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqvpwgzol.sHtML

[R66] 定时任务
来源：http://wap.fanxiaobao.xyz/Article/details/gzdpbhaoe.sHtML

crontab -e;  crontab -l
来源：http://blog.fanxiaobao.xyz/Article/details/gdcctzqfj.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.fanxiaobao.xyz/Article/details/goeccwcmh.sHtML

openssl rand -hex 16
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqywrkbuc.sHtML

[R68] 计算文件校验值
来源：http://mobile.fanxiaobao.xyz/Article/details/gjyskbqgb.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gltemjdcq.sHtML

[R69] 生成随机密码
来源：http://m.share.fanxiaobao.xyz/Article/details/gwngemcna.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdpotfoab.sHtML

[R70] 时间戳与互转
来源：http://www.blog.fanxiaobao.xyz/Article/details/gahuemwix.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.fanxiaobao.xyz/Article/details/grfrrtugc.sHtML

[R71] 日期格式化
来源：http://www.share.fanxiaobao.xyz/Article/details/gimjflcjk.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.fanxiaobao.xyz/Article/details/gqpbzsvxx.sHtML

[R72] 等待端口就绪
来源：http://3g.fanxiaobao.xyz/Article/details/gzeezvpcw.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggrvomdyb.sHtML

[R73] 分割大日志
来源：http://mobile.fanxiaobao.xyz/Article/details/ghmayukel.sHtML

split -l 1000 big.log part_
来源：http://baike.fanxiaobao.xyz/Article/details/gvlleuyep.sHtML

[R74] 批量重命名
来源：http://mobile.fanxiaobao.xyz/Article/details/gidfophky.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.fanxiaobao.xyz/Article/details/gwxlezmnl.sHtML

[R75] 导出环境变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gxwbufkeu.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.fanxiaobao.xyz/Article/details/gextdjsmm.sHtML

[R76] 使用临时文件
来源：http://blog.fanxiaobao.xyz/Article/details/grrirljmv.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.fanxiaobao.xyz/Article/details/gmithwqud.sHtML

[R77] 读取用户输入
来源：http://m.share.fanxiaobao.xyz/Article/details/gmbipwpqm.sHtML

read -rp "请输入: " ans
来源：http://m.share.fanxiaobao.xyz/Article/details/gigwwibvf.sHtML

[R78] 交互式菜单
来源：http://wap.fanxiaobao.xyz/Article/details/gzzbietfr.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.fanxiaobao.xyz/Article/details/gvlkgacmm.sHtML

[R79] 解析命令行选项
来源：http://wap.fanxiaobao.xyz/Article/details/gpztocyax.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.fanxiaobao.xyz/Article/details/ggbtbqziv.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.fanxiaobao.xyz/Article/details/ggbgxxhad.sHtML

time ./run.sh
来源：http://read.share.fanxiaobao.xyz/Article/details/gvxtmxupy.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtbnwpala.sHtML

S. C / C++ 专题
来源：http://blog.fanxiaobao.xyz/Article/details/gkdniztvu.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gzvzemdab.sHtML

[S01] C：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gtnnccmtu.sHtML

#include <stdio.h>
来源：http://www.blog.fanxiaobao.xyz/Article/details/gctlavvub.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.fanxiaobao.xyz/Article/details/gntiyrhmc.sHtML

[S02] C：变量与格式化输出
来源：http://3g.fanxiaobao.xyz/Article/details/gszewwnqp.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.fanxiaobao.xyz/Article/details/gnnnyvjbt.sHtML

[S03] C：读入整数
来源：http://mobile.fanxiaobao.xyz/Article/details/geqjameya.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqvmejnvy.sHtML

[S04] C：字符串复制
来源：http://3g.fanxiaobao.xyz/Article/details/grstqogpp.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.fanxiaobao.xyz/Article/details/grjybgvmp.sHtML

[S05] C：字符串长度
来源：http://baike.fanxiaobao.xyz/Article/details/gwekybhyk.sHtML

strlen(s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdktvoblf.sHtML

[S06] C：字符串比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/genkzweho.sHtML

strcmp(a, b) == 0
来源：http://baike.fanxiaobao.xyz/Article/details/gsfcrlafy.sHtML

[S07] C：数组遍历求和
来源：http://baike.fanxiaobao.xyz/Article/details/grfdmuina.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.fanxiaobao.xyz/Article/details/gfpiafwgk.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.fanxiaobao.xyz/Article/details/geoytfbxj.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.fanxiaobao.xyz/Article/details/gpxnargoc.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtzogjqqo.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.fanxiaobao.xyz/Article/details/gpviuhlus.sHtML

[S10] C：指针与解引用
来源：http://wap.fanxiaobao.xyz/Article/details/gbmzogdio.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.fanxiaobao.xyz/Article/details/glvkafwvn.sHtML

[S11] C：逐行读文件
来源：http://3g.fanxiaobao.xyz/Article/details/gveyriema.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.fanxiaobao.xyz/Article/details/gypuvmmsp.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.fanxiaobao.xyz/Article/details/gzlgrtjke.sHtML

fclose(f);
来源：http://blog.fanxiaobao.xyz/Article/details/ghchgdzdi.sHtML

[S12] C：写文件
来源：http://m.share.fanxiaobao.xyz/Article/details/grozjvlst.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.fanxiaobao.xyz/Article/details/gvrlbxsnw.sHtML

[S13] C：宏定义
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtddnqomw.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.fanxiaobao.xyz/Article/details/gkvplkmro.sHtML

[S14] C：枚举
来源：http://wap.fanxiaobao.xyz/Article/details/gswmitbmk.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.fanxiaobao.xyz/Article/details/gzyqhfbcx.sHtML

[S15] C：类型转换
来源：http://3g.fanxiaobao.xyz/Article/details/grasbpcwb.sHtML

(double) a / b
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggskdbgoj.sHtML

[S16] C：位操作置位
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmoekqdpi.sHtML

x |= (1 << 3);
来源：http://mobile.fanxiaobao.xyz/Article/details/gwdzsynhb.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/gbmyosqrs.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.fanxiaobao.xyz/Article/details/gyqpptplt.sHtML

[S18] C：命令行参数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goffycwdu.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdlsyower.sHtML

[S19] C：快速排序
来源：http://read.share.fanxiaobao.xyz/Article/details/gxzhnzvbi.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.fanxiaobao.xyz/Article/details/gbpnlgyjs.sHtML

[S20] C：二分查找
来源：http://3g.fanxiaobao.xyz/Article/details/gguvsqrjv.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmzafowwz.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghcpckdli.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.fanxiaobao.xyz/Article/details/gatxbtlyw.sHtML

[S22] C：字符串转数字
来源：http://3g.fanxiaobao.xyz/Article/details/giqqjfoss.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.fanxiaobao.xyz/Article/details/gfavmgonz.sHtML

[S23] C：随机数
来源：http://mobile.fanxiaobao.xyz/Article/details/gshlngcvo.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.fanxiaobao.xyz/Article/details/gxzljgiuv.sHtML

[S24] C：获取本地时间
来源：http://3g.fanxiaobao.xyz/Article/details/gtbfcaqlw.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.fanxiaobao.xyz/Article/details/ggxqcqwcf.sHtML

[S25] C：内存拷贝
来源：http://baike.fanxiaobao.xyz/Article/details/gfgooxqgb.sHtML

memcpy(dst, src, n);
来源：http://m.share.fanxiaobao.xyz/Article/details/gtiijlkpi.sHtML

[S26] C：内存清零
来源：http://mobile.fanxiaobao.xyz/Article/details/gpokyueon.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkjhwcjsh.sHtML

[S27] C：定义常量
来源：http://wap.fanxiaobao.xyz/Article/details/gqwzzpurm.sHtML

const double PI = 3.14159;
来源：http://www.share.fanxiaobao.xyz/Article/details/galmmobcf.sHtML

[S28] C：静态变量
来源：http://wap.fanxiaobao.xyz/Article/details/guwktcmcu.sHtML

static int counter = 0;
来源：http://3g.fanxiaobao.xyz/Article/details/gpcaimteg.sHtML

[S29] C：变参函数
来源：http://blog.fanxiaobao.xyz/Article/details/gsxcqglai.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwcvolirx.sHtML

[S30] C：头文件保护
来源：http://3g.fanxiaobao.xyz/Article/details/gzvzpmnid.sHtML

#ifndef X_H
来源：http://baike.fanxiaobao.xyz/Article/details/gltmdwwaw.sHtML

#define X_H
来源：http://3g.fanxiaobao.xyz/Article/details/gqiivpoja.sHtML

#endif
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqscbjbqo.sHtML

[S31] C++：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjkrjegln.sHtML

#include <iostream>
来源：http://www.share.fanxiaobao.xyz/Article/details/gimvjzijj.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqztwgvwh.sHtML

[S32] C++：字符串
来源：http://wap.fanxiaobao.xyz/Article/details/gvxsyeiuw.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.fanxiaobao.xyz/Article/details/gmzmokluj.sHtML

[S33] C++：vector 增删
来源：http://mobile.fanxiaobao.xyz/Article/details/gdtpdxkbs.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.fanxiaobao.xyz/Article/details/gpqitdkhl.sHtML

[S34] C++：遍历 vector
来源：http://mobile.fanxiaobao.xyz/Article/details/gfsqubtog.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gtqgdcmmf.sHtML

[S35] C++：map
来源：http://read.share.fanxiaobao.xyz/Article/details/gycdxxwuw.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqsvprdav.sHtML

[S36] C++：unordered_map
来源：http://mobile.fanxiaobao.xyz/Article/details/gmrqvqdyi.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/gnocsunno.sHtML

[S37] C++：set
来源：http://3g.fanxiaobao.xyz/Article/details/gaqfgoulc.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.fanxiaobao.xyz/Article/details/ggsbegdne.sHtML

[S38] C++：排序
来源：http://3g.fanxiaobao.xyz/Article/details/gjqtnygjp.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.fanxiaobao.xyz/Article/details/gaxkifvxf.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.fanxiaobao.xyz/Article/details/gythzyubr.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.fanxiaobao.xyz/Article/details/grpafwjqy.sHtML

[S40] C++：查找元素
来源：http://baike.fanxiaobao.xyz/Article/details/gtsltsrck.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.fanxiaobao.xyz/Article/details/gafmxgkbg.sHtML

[S41] C++：类与构造函数
来源：http://www.share.fanxiaobao.xyz/Article/details/ggvzcxitp.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.fanxiaobao.xyz/Article/details/ghbdybsle.sHtML

[S42] C++：继承与虚函数
来源：http://wap.fanxiaobao.xyz/Article/details/gixtvqhja.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.fanxiaobao.xyz/Article/details/gjjkucojz.sHtML

[S43] C++：智能指针
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzfzvracr.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.fanxiaobao.xyz/Article/details/gvwpomkfy.sHtML

[S44] C++：引用传参
来源：http://blog.fanxiaobao.xyz/Article/details/gzkeoynrn.sHtML

void inc(int &x) { ++x; }
来源：http://blog.fanxiaobao.xyz/Article/details/gahabyikq.sHtML

[S45] C++：lambda
来源：http://read.share.fanxiaobao.xyz/Article/details/gtiqtehct.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.fanxiaobao.xyz/Article/details/ghlfjyhnh.sHtML

[S46] C++：函数模板
来源：http://blog.fanxiaobao.xyz/Article/details/gyyzifhcb.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gdesetzui.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gometgpoo.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.fanxiaobao.xyz/Article/details/gzhzsujsn.sHtML

[S48] C++：逐行读文件
来源：http://baike.fanxiaobao.xyz/Article/details/gyfvvucuy.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.fanxiaobao.xyz/Article/details/gywmqfszi.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfxfrngwa.sHtML

[S49] C++：写文件
来源：http://www.share.fanxiaobao.xyz/Article/details/garntwaut.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmzuzomdu.sHtML

[S50] C++：格式化数字
来源：http://3g.fanxiaobao.xyz/Article/details/ghxpdywhc.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.fanxiaobao.xyz/Article/details/gccdrvybw.sHtML

[S51] C++：显式类型转换
来源：http://blog.fanxiaobao.xyz/Article/details/guariouqk.sHtML

static_cast<double>(a) / b
来源：http://wap.fanxiaobao.xyz/Article/details/gfjdoxxsd.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.fanxiaobao.xyz/Article/details/gqetognso.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gkvfxscij.sHtML

[S53] C++：移动语义
来源：http://m.share.fanxiaobao.xyz/Article/details/gnsfxuzmz.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.fanxiaobao.xyz/Article/details/ghmuffvjb.sHtML

[S54] C++：异常处理
来源：http://www.share.fanxiaobao.xyz/Article/details/giizohgkn.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.fanxiaobao.xyz/Article/details/gubeilkrs.sHtML

[S55] C++：结构化绑定
来源：http://www.share.fanxiaobao.xyz/Article/details/gskyjcyvb.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.fanxiaobao.xyz/Article/details/gtaxkuefb.sHtML

[S56] C++：optional
来源：http://mobile.fanxiaobao.xyz/Article/details/gyezrwbep.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.fanxiaobao.xyz/Article/details/grdnlrxjy.sHtML

[S57] C++：编译期常量
来源：http://www.share.fanxiaobao.xyz/Article/details/ggvghmvbm.sHtML

constexpr int N = 10;
来源：http://wap.fanxiaobao.xyz/Article/details/grhoeygwm.sHtML

[S58] C++：命名空间
来源：http://m.share.fanxiaobao.xyz/Article/details/gbsvmtijj.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.fanxiaobao.xyz/Article/details/grroogoru.sHtML

[S59] C++：静态断言
来源：http://mobile.fanxiaobao.xyz/Article/details/gxntizjww.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.fanxiaobao.xyz/Article/details/gqfpaonaw.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.fanxiaobao.xyz/Article/details/glyrqptui.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.fanxiaobao.xyz/Article/details/gnqxhpktu.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gffphttfr.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.fanxiaobao.xyz/Article/details/gkkyphinu.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gearucxxg.sHtML

[T01] Kotlin：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/grfqeuqrf.sHtML

println("Hello")
来源：http://baike.fanxiaobao.xyz/Article/details/ghzlbefdj.sHtML

[T02] Kotlin：变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gzanhycry.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.fanxiaobao.xyz/Article/details/grcuegenf.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.fanxiaobao.xyz/Article/details/gmdmzspur.sHtML

"值: $b"
来源：http://mobile.fanxiaobao.xyz/Article/details/gvivralbt.sHtML

[T04] Kotlin：空安全
来源：http://mobile.fanxiaobao.xyz/Article/details/gzwyjqlcb.sHtML

val n: String? = null;  n?.length
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdtocognh.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjxajxoya.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwfgnladf.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.fanxiaobao.xyz/Article/details/gqomxfrfs.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.fanxiaobao.xyz/Article/details/gktutvysk.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gapxlddhd.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.fanxiaobao.xyz/Article/details/glhfnarhc.sHtML

[T08] Kotlin：数据类
来源：http://read.share.fanxiaobao.xyz/Article/details/gzrgskkpn.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gidxuunqg.sHtML

[T09] Kotlin：扩展函数
来源：http://blog.fanxiaobao.xyz/Article/details/gcsccrmgc.sHtML

fun String.exclaim() = this + "!"
来源：http://wap.fanxiaobao.xyz/Article/details/glyxoomee.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.fanxiaobao.xyz/Article/details/getjhbmgr.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.fanxiaobao.xyz/Article/details/gxsnonucr.sHtML

[T11] Kotlin：协程
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvjgljakl.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.fanxiaobao.xyz/Article/details/gsdzihovm.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.fanxiaobao.xyz/Article/details/gnfzzdlmq.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/geychfoll.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.fanxiaobao.xyz/Article/details/guzorlacp.sHtML

val m = mapOf("a" to 1)
来源：http://3g.fanxiaobao.xyz/Article/details/gaewszabs.sHtML

[T14] Kotlin：循环
来源：http://3g.fanxiaobao.xyz/Article/details/gcthjkzbm.sHtML

for (i in 1..10) println(i)
来源：http://3g.fanxiaobao.xyz/Article/details/gxkagkjpl.sHtML

[T15] Kotlin：接口
来源：http://read.share.fanxiaobao.xyz/Article/details/gluaulect.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.fanxiaobao.xyz/Article/details/gsjaujhpj.sHtML

[T16] Swift：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gpkkobspp.sHtML

print("Hello")
来源：http://3g.fanxiaobao.xyz/Article/details/grtomtdcu.sHtML

[T17] Swift：变量与常量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gftexnyml.sHtML

var a = 1;  let b = 2
来源：http://3g.fanxiaobao.xyz/Article/details/ghmtdmtou.sHtML

[T18] Swift：字符串插值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggfddvnck.sHtML

"值: \(b)"
来源：http://read.share.fanxiaobao.xyz/Article/details/gqbiqpfrd.sHtML

[T19] Swift：可选绑定
来源：http://wap.fanxiaobao.xyz/Article/details/ghrcdcxhy.sHtML

if let n = opt { print(n) }
来源：http://m.share.fanxiaobao.xyz/Article/details/gbgxdpony.sHtML

[T20] Swift：数组操作
来源：http://3g.fanxiaobao.xyz/Article/details/gutmtoyte.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://blog.fanxiaobao.xyz/Article/details/gzkfkoggw.sHtML

[T21] Swift：遍历
来源：http://mobile.fanxiaobao.xyz/Article/details/gsehtjauf.sHtML

for x in a { print(x) }
来源：http://wap.fanxiaobao.xyz/Article/details/ghspozpsx.sHtML

[T22] Swift：字典
来源：http://read.share.fanxiaobao.xyz/Article/details/gexfjpzzk.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://3g.fanxiaobao.xyz/Article/details/gtvwkzgzz.sHtML

[T23] Swift：函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gusejowqt.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.fanxiaobao.xyz/Article/details/gqfujliiw.sHtML

[T24] Swift：闭包
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gplwpbctj.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://read.share.fanxiaobao.xyz/Article/details/gnpwxbrnu.sHtML

[T25] Swift：结构体
来源：http://m.share.fanxiaobao.xyz/Article/details/gnsbijvbr.sHtML

struct P { var x: Int }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxzseywjb.sHtML

[T26] Swift：类与重写
来源：http://blog.fanxiaobao.xyz/Article/details/ganppyukj.sHtML

class A: Base { override func f() {} }
来源：http://www.blog.fanxiaobao.xyz/Article/details/giwbsmvoj.sHtML

[T27] Swift：错误处理
来源：http://blog.fanxiaobao.xyz/Article/details/glxdxsyiy.sHtML

do { try f() } catch { print(error) }
来源：http://www.share.fanxiaobao.xyz/Article/details/gbicjlwcm.sHtML

[T28] Swift：枚举
来源：http://wap.fanxiaobao.xyz/Article/details/gyiiikkfv.sHtML

enum Color { case red, green }
来源：http://3g.fanxiaobao.xyz/Article/details/gtxsfcynv.sHtML

[T29] Swift：guard 提前返回
来源：http://3g.fanxiaobao.xyz/Article/details/grlzxqifq.sHtML

guard let x = opt else { return }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gihxagqrj.sHtML

[T30] Swift：协议
来源：http://www.blog.fanxiaobao.xyz/Article/details/gipfhbprn.sHtML

protocol Shape { func area() -> Double }
来源：http://mobile.fanxiaobao.xyz/Article/details/gcdquzprg.sHtML


<!-- 参考信息 -->