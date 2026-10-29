代发 wailian999

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.hesvh.cn/Article/details/gugkpdetb.sHtML

[R10] 正则匹配
来源：http://www.blog.hesvh.cn/Article/details/gtrdlhqbp.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.hesvh.cn/Article/details/gzizhxisb.sHtML

[R11] case 多分支
来源：http://www.share.hesvh.cn/Article/details/gvxlljabw.sHtML

case "$1" in
来源：http://read.share.hesvh.cn/Article/details/gvqpgxlii.sHtML

start) echo "启动" ;;
来源：http://wap.zdbjq.cn/Article/details/gavfgrykd.sHtML

stop)  echo "停止" ;;
来源：http://mobile.zdbjq.cn/Article/details/gcbvvawrl.sHtML

*)     echo "未知命令" ;;
来源：http://3g.fehbvm.com/Article/details/gebcvvrkg.sHtML

esac
来源：http://baike.zdbjq.cn/Article/details/giickzfkm.sHtML

[R12] for 遍历文件
来源：http://mobile.hesvh.cn/Article/details/gmrqhbhru.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.fehbvm.com/Article/details/gelspilcz.sHtML

[R13] for 计数循环
来源：http://read.share.fehbvm.com/Article/details/gocgrewxn.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.zdbjq.cn/Article/details/glasqegub.sHtML

[R14] C 风格 for
来源：http://blog.fehbvm.com/Article/details/gdyxyyjxa.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.hesvh.cn/Article/details/gbbypmznr.sHtML

[R15] while 逐行读文件
来源：http://m.share.hesvh.cn/Article/details/gdguzpsky.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.zdbjq.cn/Article/details/gfzjdkzyp.sHtML

[R16] until 等待条件
来源：http://www.share.fehbvm.com/Article/details/gaapslixj.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.fehbvm.com/Article/details/gyxidcflg.sHtML

[R17] 数组定义与取值
来源：http://3g.hesvh.cn/Article/details/ghgwybhyh.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://wap.fehbvm.com/Article/details/gmpxeepcn.sHtML

[R18] 遍历数组
来源：http://www.blog.hesvh.cn/Article/details/guwchmgay.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.m.share.hesvh.cn/Article/details/gofcbbavq.sHtML

[R19] 数组长度
来源：http://read.share.hesvh.cn/Article/details/gazmumldc.sHtML

echo "${#arr[@]}"
来源：http://blog.zdbjq.cn/Article/details/gqwbpgbmg.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.zdbjq.cn/Article/details/grahpiikp.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.hesvh.cn/Article/details/gwulwhekd.sHtML

[R21] 字符串长度
来源：http://www.m.share.hesvh.cn/Article/details/gjtjjlgzv.sHtML

echo "${#s}"
来源：http://baike.hesvh.cn/Article/details/gpsjninjn.sHtML

[R22] 截取子串
来源：http://mobile.zdbjq.cn/Article/details/gubrbokka.sHtML

echo "${s:0:5}"
来源：http://baike.hesvh.cn/Article/details/gfoqsyeeb.sHtML

[R23] 字符串替换
来源：http://3g.zdbjq.cn/Article/details/gfgrfomef.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.hesvh.cn/Article/details/gbwoiqizx.sHtML

[R24] 大小写转换
来源：http://wap.zdbjq.cn/Article/details/gfqknnptc.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.fehbvm.com/Article/details/gfztinzpu.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.zdbjq.cn/Article/details/gdvjjfung.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.hesvh.cn/Article/details/gikrpcnqe.sHtML

[R26] 命令替换
来源：http://read.share.zdbjq.cn/Article/details/gjwabwfdq.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.hesvh.cn/Article/details/gimurmjjq.sHtML

[R27] 算术展开
来源：http://www.m.share.fehbvm.com/Article/details/gcvxubtkc.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.fehbvm.com/Article/details/gjlvokirj.sHtML

[R28] 浮点运算
来源：http://wap.hesvh.cn/Article/details/gdefgrexs.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.hesvh.cn/Article/details/gicwjgttn.sHtML

[R29] 定义函数
来源：http://wap.hesvh.cn/Article/details/gnhbfovsr.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.zdbjq.cn/Article/details/gpdopmcpk.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.zdbjq.cn/Article/details/gbsyqvjte.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.hesvh.cn/Article/details/gstyewtqp.sHtML

[R31] 局部变量
来源：http://www.share.hesvh.cn/Article/details/gwsfmzfos.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.fehbvm.com/Article/details/gazubyglp.sHtML

[R32] 参数个数校验
来源：http://baike.hesvh.cn/Article/details/gqinrumnp.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.hesvh.cn/Article/details/gpmgoomte.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.zdbjq.cn/Article/details/glbuuqimq.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.hesvh.cn/Article/details/gccxlrvfx.sHtML

[R34] 退出时清理
来源：http://baike.hesvh.cn/Article/details/gyzfcpexd.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fehbvm.com/Article/details/gmgblmwtz.sHtML

[R35] 后台执行并等待
来源：http://www.share.fehbvm.com/Article/details/gvdoafuxc.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://3g.hesvh.cn/Article/details/gwxzpzaxs.sHtML

[R36] 并发执行多个任务
来源：http://3g.zdbjq.cn/Article/details/glpqodtsr.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.hesvh.cn/Article/details/guctcmpaj.sHtML

[R37] 把输出赋给变量
来源：http://wap.zdbjq.cn/Article/details/gylpbpkxg.sHtML

files=$(ls -1)
来源：http://3g.zdbjq.cn/Article/details/gnqvtmiiw.sHtML

[R38] 管道串联
来源：http://read.share.hesvh.cn/Article/details/giuthxltd.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.fehbvm.com/Article/details/geleigqxm.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.hesvh.cn/Article/details/getsriozv.sHtML

cmd > out.log 2>&1
来源：http://www.share.fehbvm.com/Article/details/gwnonmfgb.sHtML

[R40] 追加写日志
来源：http://www.m.share.hesvh.cn/Article/details/gwilotxgp.sHtML

echo "log" >> out.log
来源：http://blog.fehbvm.com/Article/details/gudkjtilq.sHtML

[R41] 丢弃输出
来源：http://baike.fehbvm.com/Article/details/glxmeffnn.sHtML

cmd >/dev/null 2>&1
来源：http://wap.hesvh.cn/Article/details/gakiiydgm.sHtML

[R42] 输入重定向
来源：http://m.share.hesvh.cn/Article/details/grfvykvbd.sHtML

wc -l < a.txt
来源：http://mobile.zdbjq.cn/Article/details/gzdixyucu.sHtML

[R43] 按名字查找文件
来源：http://www.share.zdbjq.cn/Article/details/gtvtorijw.sHtML

find . -name "*.log" -type f
来源：http://blog.zdbjq.cn/Article/details/gusrvoluq.sHtML

[R44] 按修改时间查找
来源：http://mobile.zdbjq.cn/Article/details/gubtkadux.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.zdbjq.cn/Article/details/ggqryfchp.sHtML

[R45] 批量删除
来源：http://mobile.zdbjq.cn/Article/details/goomfczmv.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.zdbjq.cn/Article/details/gdcfcmkxv.sHtML

[R46] 递归替换文件内容
来源：http://wap.fehbvm.com/Article/details/gseuwxkcb.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.zdbjq.cn/Article/details/gnvcnuqxk.sHtML

[R47] sed 单行替换
来源：http://m.share.fehbvm.com/Article/details/gllksaopa.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.fehbvm.com/Article/details/getsvahfh.sHtML

[R48] awk 取指定列
来源：http://read.share.zdbjq.cn/Article/details/gxrjzpvnf.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.zdbjq.cn/Article/details/guvcsdgzi.sHtML

[R49] awk 带条件
来源：http://read.share.hesvh.cn/Article/details/gwslgsjfp.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.fehbvm.com/Article/details/ghpzlwneu.sHtML

[R50] awk 求和
来源：http://3g.zdbjq.cn/Article/details/gvwrkqebn.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.hesvh.cn/Article/details/gtuhwxvcg.sHtML

[R51] 排序去重取前几
来源：http://3g.hesvh.cn/Article/details/gtlxsrunx.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.fehbvm.com/Article/details/ghqzjpgbe.sHtML

[R52] 统计行数
来源：http://baike.hesvh.cn/Article/details/gbacysuus.sHtML

wc -l a.txt
来源：http://mobile.hesvh.cn/Article/details/gicaqpdmo.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.zdbjq.cn/Article/details/gxmokoeqd.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.fehbvm.com/Article/details/gsmtusylw.sHtML

[R54] 比较两个文件
来源：http://read.share.zdbjq.cn/Article/details/gjzfjcxsv.sHtML

diff a.txt b.txt
来源：http://www.share.hesvh.cn/Article/details/gtyizxzlx.sHtML

[R55] 压缩与解压
来源：http://wap.fehbvm.com/Article/details/gghaghqml.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.fehbvm.com/Article/details/gkcpujltc.sHtML

[R56] 远程拷贝
来源：http://www.share.hesvh.cn/Article/details/gptvppwxy.sHtML

scp file user@host:/path/
来源：http://www.blog.zdbjq.cn/Article/details/ghheyimwm.sHtML

[R57] 远程执行命令
来源：http://www.blog.hesvh.cn/Article/details/gzgenolmf.sHtML

ssh user@host 'uptime'
来源：http://www.share.hesvh.cn/Article/details/gsxfsojwa.sHtML

[R58] 下载文件
来源：http://m.share.zdbjq.cn/Article/details/gswlhqlgq.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.zdbjq.cn/Article/details/gwmklnzjn.sHtML

[R59] 发 POST JSON
来源：http://wap.zdbjq.cn/Article/details/gweuesuzi.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.fehbvm.com/Article/details/gkmvccyfo.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.hesvh.cn/Article/details/gbsxshdpm.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.fehbvm.com/Article/details/gvqgyddtc.sHtML

[R61] 磁盘占用
来源：http://www.blog.fehbvm.com/Article/details/gxxlhbhku.sHtML

df -h;  du -sh *
来源：http://www.share.fehbvm.com/Article/details/gsfidqugj.sHtML

[R62] 找最占空间的文件
来源：http://read.share.fehbvm.com/Article/details/grpmemezq.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.fehbvm.com/Article/details/gkfhhsmiw.sHtML

[R63] 内存与进程
来源：http://m.share.fehbvm.com/Article/details/grvjvyajv.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.fehbvm.com/Article/details/gagdrwljt.sHtML

[R64] 结束进程
来源：http://3g.hesvh.cn/Article/details/gktpwvczl.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.fehbvm.com/Article/details/gyrysfacn.sHtML

[R65] 查看端口占用
来源：http://read.share.hesvh.cn/Article/details/gfycaeofm.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.fehbvm.com/Article/details/gbwutvhbj.sHtML

[R66] 定时任务
来源：http://3g.fehbvm.com/Article/details/gzftwxzbl.sHtML

crontab -e;  crontab -l
来源：http://3g.zdbjq.cn/Article/details/glrcuhiad.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.zdbjq.cn/Article/details/ghfmchdxe.sHtML

openssl rand -hex 16
来源：http://3g.zdbjq.cn/Article/details/gwnclahlg.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.zdbjq.cn/Article/details/ghmheekdx.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.zdbjq.cn/Article/details/gkvijkrdg.sHtML

[R69] 生成随机密码
来源：http://read.share.hesvh.cn/Article/details/glkmwlgjd.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.fehbvm.com/Article/details/gzruoaall.sHtML

[R70] 时间戳与互转
来源：http://3g.hesvh.cn/Article/details/gsimlivdk.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.fehbvm.com/Article/details/gflydfcbc.sHtML

[R71] 日期格式化
来源：http://blog.hesvh.cn/Article/details/gocornxrx.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.hesvh.cn/Article/details/gsvifwlqt.sHtML

[R72] 等待端口就绪
来源：http://www.share.fehbvm.com/Article/details/gvpbhbulo.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.fehbvm.com/Article/details/goieqlnot.sHtML

[R73] 分割大日志
来源：http://baike.fehbvm.com/Article/details/geqdpxlkp.sHtML

split -l 1000 big.log part_
来源：http://3g.fehbvm.com/Article/details/gvgkgzqiz.sHtML

[R74] 批量重命名
来源：http://www.blog.fehbvm.com/Article/details/gqllqtorm.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.fehbvm.com/Article/details/gjpgpssji.sHtML

[R75] 导出环境变量
来源：http://www.blog.fehbvm.com/Article/details/guixvhlio.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.fehbvm.com/Article/details/gcuclszvt.sHtML

[R76] 使用临时文件
来源：http://blog.zdbjq.cn/Article/details/gjfifihft.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.fehbvm.com/Article/details/gwimbkper.sHtML

[R77] 读取用户输入
来源：http://3g.fehbvm.com/Article/details/gbcdpegzp.sHtML

read -rp "请输入: " ans
来源：http://www.share.fehbvm.com/Article/details/gmphuqvik.sHtML

[R78] 交互式菜单
来源：http://www.blog.zdbjq.cn/Article/details/gfdqpzcvq.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.hesvh.cn/Article/details/gxjztmhsk.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.fehbvm.com/Article/details/geyjaxnrc.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.hesvh.cn/Article/details/gumzktjpm.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.fehbvm.com/Article/details/gvehewtfy.sHtML

time ./run.sh
来源：http://mobile.hesvh.cn/Article/details/gokkowwul.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gsduypihw.sHtML

S. C / C++ 专题
来源：http://mobile.zdbjq.cn/Article/details/gobgwpenm.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gpmhbiaqy.sHtML

[S01] C：Hello World
来源：http://baike.zdbjq.cn/Article/details/gsuvdwjuu.sHtML

#include <stdio.h>
来源：http://baike.zdbjq.cn/Article/details/gcyvzrfqn.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.fehbvm.com/Article/details/gkwyjmfon.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.hesvh.cn/Article/details/gnihgbmlv.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.hesvh.cn/Article/details/gqgyvhisj.sHtML

[S03] C：读入整数
来源：http://www.share.zdbjq.cn/Article/details/gqlioksyr.sHtML

int x; scanf("%d", &x);
来源：http://read.share.fehbvm.com/Article/details/gdfpyjicr.sHtML

[S04] C：字符串复制
来源：http://mobile.hesvh.cn/Article/details/gweeyrkoh.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.zdbjq.cn/Article/details/gjnuysqio.sHtML

[S05] C：字符串长度
来源：http://blog.hesvh.cn/Article/details/gaqaoxlcs.sHtML

strlen(s)
来源：http://www.share.zdbjq.cn/Article/details/gaglxyhab.sHtML

[S06] C：字符串比较
来源：http://mobile.hesvh.cn/Article/details/guhmiswfv.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.zdbjq.cn/Article/details/goucsxopo.sHtML

[S07] C：数组遍历求和
来源：http://3g.zdbjq.cn/Article/details/gfbpziscx.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.zdbjq.cn/Article/details/gizaezjcg.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.zdbjq.cn/Article/details/gxpuvmdsd.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.zdbjq.cn/Article/details/gzfnjdayp.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.fehbvm.com/Article/details/gccdnxrmx.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.fehbvm.com/Article/details/gtaidknqs.sHtML

[S10] C：指针与解引用
来源：http://www.blog.hesvh.cn/Article/details/gkyfribzd.sHtML

int *p = &a;  *p = 5;
来源：http://wap.zdbjq.cn/Article/details/gpbnnlndo.sHtML

[S11] C：逐行读文件
来源：http://www.blog.zdbjq.cn/Article/details/gizgjggof.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.hesvh.cn/Article/details/gniljydki.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.hesvh.cn/Article/details/gbjhtitvm.sHtML

fclose(f);
来源：http://read.share.fehbvm.com/Article/details/gmrsyufxm.sHtML

[S12] C：写文件
来源：http://mobile.hesvh.cn/Article/details/ggucywwew.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.hesvh.cn/Article/details/gmmhnhnrg.sHtML

[S13] C：宏定义
来源：http://read.share.fehbvm.com/Article/details/gspmsukcm.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.zdbjq.cn/Article/details/gzqhotxoo.sHtML

[S14] C：枚举
来源：http://www.share.fehbvm.com/Article/details/ghqvjnihp.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.zdbjq.cn/Article/details/gpaebyxwr.sHtML

[S15] C：类型转换
来源：http://www.blog.fehbvm.com/Article/details/gbhxwzhhs.sHtML

(double) a / b
来源：http://mobile.hesvh.cn/Article/details/gjjnkaeme.sHtML

[S16] C：位操作置位
来源：http://baike.hesvh.cn/Article/details/gniynvmfu.sHtML

x |= (1 << 3);
来源：http://3g.zdbjq.cn/Article/details/gaxbnpwfp.sHtML

[S17] C：安全拼接字符串
来源：http://3g.fehbvm.com/Article/details/gzlotxkhg.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.fehbvm.com/Article/details/gxztuvlrf.sHtML

[S18] C：命令行参数
来源：http://www.blog.hesvh.cn/Article/details/gztiiiyjs.sHtML

int main(int argc, char **argv)
来源：http://www.blog.zdbjq.cn/Article/details/genptvslb.sHtML

[S19] C：快速排序
来源：http://www.blog.fehbvm.com/Article/details/geunqvwjl.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.fehbvm.com/Article/details/giikdrsvm.sHtML

[S20] C：二分查找
来源：http://m.share.hesvh.cn/Article/details/gyaxyqbuh.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.hesvh.cn/Article/details/guuerhqzx.sHtML

[S21] C：字符类别判断
来源：http://www.blog.zdbjq.cn/Article/details/gakzcpuui.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.hesvh.cn/Article/details/gmfrmmpak.sHtML

[S22] C：字符串转数字
来源：http://baike.hesvh.cn/Article/details/gavdyoyyu.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.fehbvm.com/Article/details/gliczmjry.sHtML

[S23] C：随机数
来源：http://3g.hesvh.cn/Article/details/gghmvwiyh.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.fehbvm.com/Article/details/gajpqgzbn.sHtML

[S24] C：获取本地时间
来源：http://baike.fehbvm.com/Article/details/ghtjdmgis.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.fehbvm.com/Article/details/gvfvmxmvb.sHtML

[S25] C：内存拷贝
来源：http://mobile.fehbvm.com/Article/details/gmdxbqurl.sHtML

memcpy(dst, src, n);
来源：http://m.share.zdbjq.cn/Article/details/gbskipixe.sHtML

[S26] C：内存清零
来源：http://www.m.share.hesvh.cn/Article/details/gmlmxudyu.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.hesvh.cn/Article/details/gsymkfpbe.sHtML

[S27] C：定义常量
来源：http://3g.hesvh.cn/Article/details/gzazueeej.sHtML

const double PI = 3.14159;
来源：http://m.share.fehbvm.com/Article/details/gbnlpykxx.sHtML

[S28] C：静态变量
来源：http://wap.zdbjq.cn/Article/details/gdukkmycr.sHtML

static int counter = 0;
来源：http://wap.zdbjq.cn/Article/details/gbbubzuss.sHtML

[S29] C：变参函数
来源：http://www.share.fehbvm.com/Article/details/gyacwesfr.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.zdbjq.cn/Article/details/gqpbkpkwt.sHtML

[S30] C：头文件保护
来源：http://mobile.zdbjq.cn/Article/details/gzjvugwjg.sHtML

#ifndef X_H
来源：http://baike.zdbjq.cn/Article/details/gublhhpsj.sHtML

#define X_H
来源：http://wap.fehbvm.com/Article/details/gohlqxbsh.sHtML

#endif
来源：http://mobile.hesvh.cn/Article/details/ghrardirl.sHtML

[S31] C++：Hello World
来源：http://www.share.fehbvm.com/Article/details/gumhrvydb.sHtML

#include <iostream>
来源：http://www.share.zdbjq.cn/Article/details/gowtunatb.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.zdbjq.cn/Article/details/ghrqoarbc.sHtML

[S32] C++：字符串
来源：http://3g.zdbjq.cn/Article/details/guwbapfop.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.fehbvm.com/Article/details/ghguytvvj.sHtML

[S33] C++：vector 增删
来源：http://baike.hesvh.cn/Article/details/gwpgrqcdh.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.hesvh.cn/Article/details/gqqjvxmfk.sHtML

[S34] C++：遍历 vector
来源：http://m.share.hesvh.cn/Article/details/gdkryktdb.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.fehbvm.com/Article/details/gyfsmtrmt.sHtML

[S35] C++：map
来源：http://read.share.hesvh.cn/Article/details/gsxmjtvby.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.hesvh.cn/Article/details/gyxzpeqta.sHtML

[S36] C++：unordered_map
来源：http://baike.fehbvm.com/Article/details/ghenumwep.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.hesvh.cn/Article/details/gehovmnvo.sHtML

[S37] C++：set
来源：http://m.share.hesvh.cn/Article/details/gkyoodcgo.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.hesvh.cn/Article/details/gmymjivzn.sHtML

[S38] C++：排序
来源：http://m.share.hesvh.cn/Article/details/gcqcytxub.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.fehbvm.com/Article/details/ghevdzfez.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.zdbjq.cn/Article/details/ghmewodct.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.fehbvm.com/Article/details/gxoqgnjin.sHtML

[S40] C++：查找元素
来源：http://www.share.zdbjq.cn/Article/details/gyjyaoldf.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.zdbjq.cn/Article/details/gprhqucqj.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.hesvh.cn/Article/details/geqybzsfc.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.zdbjq.cn/Article/details/gwcqcuwjg.sHtML

[S42] C++：继承与虚函数
来源：http://mobile.fehbvm.com/Article/details/goerjgcgw.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.fehbvm.com/Article/details/gpwjsvtxf.sHtML

[S43] C++：智能指针
来源：http://www.blog.fehbvm.com/Article/details/gsgxhixyc.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.fehbvm.com/Article/details/gfejlfdqo.sHtML

[S44] C++：引用传参
来源：http://baike.fehbvm.com/Article/details/ggckedhbr.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.hesvh.cn/Article/details/glxtvrupi.sHtML

[S45] C++：lambda
来源：http://blog.hesvh.cn/Article/details/gjtnkiuny.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.hesvh.cn/Article/details/gdtzbwkpk.sHtML

[S46] C++：函数模板
来源：http://www.blog.zdbjq.cn/Article/details/ghjvjbtfc.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.zdbjq.cn/Article/details/goxkmzrzm.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.zdbjq.cn/Article/details/gbthhhqkv.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.zdbjq.cn/Article/details/gmgrncbwq.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.hesvh.cn/Article/details/gjsnjewdc.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.hesvh.cn/Article/details/gqldijyhx.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.hesvh.cn/Article/details/gffstofsw.sHtML

[S49] C++：写文件
来源：http://www.share.zdbjq.cn/Article/details/gcqfqlaqy.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.fehbvm.com/Article/details/gdxdsblwa.sHtML

[S50] C++：格式化数字
来源：http://baike.zdbjq.cn/Article/details/gntrvtykz.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.hesvh.cn/Article/details/gomoqumfz.sHtML

[S51] C++：显式类型转换
来源：http://read.share.hesvh.cn/Article/details/ggswrunrq.sHtML

static_cast<double>(a) / b
来源：http://blog.fehbvm.com/Article/details/gwaxvbflv.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.hesvh.cn/Article/details/gwguobhjj.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.hesvh.cn/Article/details/groobukxq.sHtML

[S53] C++：移动语义
来源：http://blog.fehbvm.com/Article/details/ghbfbovch.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.zdbjq.cn/Article/details/gbeiaqxpf.sHtML

[S54] C++：异常处理
来源：http://3g.fehbvm.com/Article/details/ghkambzlg.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.hesvh.cn/Article/details/gkrjftier.sHtML

[S55] C++：结构化绑定
来源：http://baike.zdbjq.cn/Article/details/gcafliwrk.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.zdbjq.cn/Article/details/geztzftal.sHtML

[S56] C++：optional
来源：http://blog.zdbjq.cn/Article/details/gxzozmauw.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.fehbvm.com/Article/details/ghckqwynv.sHtML

[S57] C++：编译期常量
来源：http://baike.hesvh.cn/Article/details/gqrffwluq.sHtML

constexpr int N = 10;
来源：http://www.share.zdbjq.cn/Article/details/gehlxgbwa.sHtML

[S58] C++：命名空间
来源：http://wap.hesvh.cn/Article/details/gmtkodelt.sHtML

namespace ns { int f() { return 1; } }
来源：http://read.share.zdbjq.cn/Article/details/goutcyhjw.sHtML

[S59] C++：静态断言
来源：http://blog.fehbvm.com/Article/details/gywyrysvx.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.zdbjq.cn/Article/details/gxlnxnmvi.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.hesvh.cn/Article/details/gvcafuoyz.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.m.share.fehbvm.com/Article/details/ghzhaaiyu.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gyiykqezr.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.zdbjq.cn/Article/details/gbvanwtix.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gxvnxbgvi.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gweajgcqc.sHtML

println("Hello")
来源：http://mobile.zdbjq.cn/Article/details/gwwznwwlb.sHtML

[T02] Kotlin：变量
来源：http://read.share.fehbvm.com/Article/details/goopqyzll.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.zdbjq.cn/Article/details/gdxowcxas.sHtML

[T03] Kotlin：字符串模板
来源：http://www.m.share.fehbvm.com/Article/details/gnokwlxtw.sHtML

"值: $b"
来源：http://m.share.zdbjq.cn/Article/details/gmxmjpgov.sHtML

[T04] Kotlin：空安全
来源：http://blog.fehbvm.com/Article/details/gglueptro.sHtML

val n: String? = null;  n?.length
来源：http://m.share.zdbjq.cn/Article/details/gcfkgvbgn.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.zdbjq.cn/Article/details/goinlviif.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.fehbvm.com/Article/details/gfeuauigp.sHtML

[T06] Kotlin：集合映射
来源：http://www.m.share.fehbvm.com/Article/details/gliqkzpxm.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.hesvh.cn/Article/details/gfhwxvykn.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.fehbvm.com/Article/details/gxrghxzpz.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://3g.fehbvm.com/Article/details/glhgvzhlh.sHtML

[T08] Kotlin：数据类
来源：http://www.share.fehbvm.com/Article/details/gnnnsihem.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.zdbjq.cn/Article/details/gwhjvoand.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.fehbvm.com/Article/details/ggtrqhqyy.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.fehbvm.com/Article/details/gjpraxhae.sHtML

[T10] Kotlin：默认参数
来源：http://www.m.share.fehbvm.com/Article/details/gxivwpodd.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.zdbjq.cn/Article/details/gwfrciuuz.sHtML


<!-- 参考信息 -->