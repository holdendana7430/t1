代发 wailian999

esac
来源：http://3g.fehbvm.com/Article/details/gzirzyfkv.sHtML

[R12] for 遍历文件
来源：http://www.m.share.fehbvm.com/Article/details/gltzkddeo.sHtML

for f in *.txt; do echo "$f"; done
来源：http://mobile.hesvh.cn/Article/details/gqlxmioxd.sHtML

[R13] for 计数循环
来源：http://www.blog.hesvh.cn/Article/details/ggnhjtvqw.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.zdbjq.cn/Article/details/gpcwvaebr.sHtML

[R14] C 风格 for
来源：http://3g.zdbjq.cn/Article/details/gdoggzdvp.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://baike.hesvh.cn/Article/details/gjiyqhwds.sHtML

[R15] while 逐行读文件
来源：http://baike.fehbvm.com/Article/details/gfxaulfrq.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.zdbjq.cn/Article/details/gpbaddgyn.sHtML

[R16] until 等待条件
来源：http://m.share.fehbvm.com/Article/details/gvqhsxlja.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.fehbvm.com/Article/details/grubktcic.sHtML

[R17] 数组定义与取值
来源：http://blog.fehbvm.com/Article/details/gwprkaxvc.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://3g.hesvh.cn/Article/details/gvpbusdqt.sHtML

[R18] 遍历数组
来源：http://baike.zdbjq.cn/Article/details/gkmunlcnn.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.zdbjq.cn/Article/details/grsnyzjoo.sHtML

[R19] 数组长度
来源：http://mobile.hesvh.cn/Article/details/gttexdrgs.sHtML

echo "${#arr[@]}"
来源：http://m.share.fehbvm.com/Article/details/gzywmtidk.sHtML

[R20] 关联数组（字典）
来源：http://www.share.fehbvm.com/Article/details/gehbzdqxz.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.fehbvm.com/Article/details/gaaslatzv.sHtML

[R21] 字符串长度
来源：http://mobile.fehbvm.com/Article/details/gxtzjxgmh.sHtML

echo "${#s}"
来源：http://mobile.hesvh.cn/Article/details/gykaypdxk.sHtML

[R22] 截取子串
来源：http://read.share.zdbjq.cn/Article/details/giiehbwhj.sHtML

echo "${s:0:5}"
来源：http://m.share.zdbjq.cn/Article/details/gbtykucbs.sHtML

[R23] 字符串替换
来源：http://3g.zdbjq.cn/Article/details/gzusjgcam.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.hesvh.cn/Article/details/ghqurgwms.sHtML

[R24] 大小写转换
来源：http://wap.zdbjq.cn/Article/details/gjhkohfxt.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.fehbvm.com/Article/details/ggpniksqa.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.fehbvm.com/Article/details/gtflcfzzq.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.fehbvm.com/Article/details/glsqoaheb.sHtML

[R26] 命令替换
来源：http://wap.fehbvm.com/Article/details/gxhylhher.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.fehbvm.com/Article/details/gvmntuhdh.sHtML

[R27] 算术展开
来源：http://baike.hesvh.cn/Article/details/gnnqlupkc.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.zdbjq.cn/Article/details/guddckylk.sHtML

[R28] 浮点运算
来源：http://3g.zdbjq.cn/Article/details/gmjcvspfi.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.zdbjq.cn/Article/details/gheoblpal.sHtML

[R29] 定义函数
来源：http://baike.zdbjq.cn/Article/details/gqszleqcb.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.zdbjq.cn/Article/details/gbollgfuj.sHtML

[R30] 函数返回状态码
来源：http://www.blog.fehbvm.com/Article/details/gitiexhtq.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.zdbjq.cn/Article/details/gblckrezx.sHtML

[R31] 局部变量
来源：http://mobile.fehbvm.com/Article/details/gijtwappw.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.fehbvm.com/Article/details/gwvzglglx.sHtML

[R32] 参数个数校验
来源：http://mobile.zdbjq.cn/Article/details/gkkdhzxnx.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.zdbjq.cn/Article/details/ggqopwqnt.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.hesvh.cn/Article/details/gbdyqfgac.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.zdbjq.cn/Article/details/gyibaoywh.sHtML

[R34] 退出时清理
来源：http://www.share.zdbjq.cn/Article/details/gvekdojjg.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.zdbjq.cn/Article/details/gqlumwvpm.sHtML

[R35] 后台执行并等待
来源：http://m.share.fehbvm.com/Article/details/ganlgjrxe.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.zdbjq.cn/Article/details/gcjxtttgb.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.hesvh.cn/Article/details/ggwylalgi.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.zdbjq.cn/Article/details/gqzzwvmnm.sHtML

[R37] 把输出赋给变量
来源：http://www.share.fehbvm.com/Article/details/gjjfbtuah.sHtML

files=$(ls -1)
来源：http://mobile.zdbjq.cn/Article/details/gddmihdui.sHtML

[R38] 管道串联
来源：http://mobile.zdbjq.cn/Article/details/geuhckder.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.zdbjq.cn/Article/details/gqtdeaspx.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.hesvh.cn/Article/details/gzbjpykbf.sHtML

cmd > out.log 2>&1
来源：http://blog.fehbvm.com/Article/details/gxsuexcjd.sHtML

[R40] 追加写日志
来源：http://baike.zdbjq.cn/Article/details/gqjgbzafu.sHtML

echo "log" >> out.log
来源：http://read.share.hesvh.cn/Article/details/giqqokkfd.sHtML

[R41] 丢弃输出
来源：http://read.share.zdbjq.cn/Article/details/gnmhtcbge.sHtML

cmd >/dev/null 2>&1
来源：http://www.blog.zdbjq.cn/Article/details/gqefrmvsp.sHtML

[R42] 输入重定向
来源：http://blog.zdbjq.cn/Article/details/ggmedjhqo.sHtML

wc -l < a.txt
来源：http://baike.hesvh.cn/Article/details/givkvzetc.sHtML

[R43] 按名字查找文件
来源：http://m.share.zdbjq.cn/Article/details/gmrpxnxqe.sHtML

find . -name "*.log" -type f
来源：http://m.share.fehbvm.com/Article/details/gnkrepyrl.sHtML

[R44] 按修改时间查找
来源：http://baike.fehbvm.com/Article/details/gxtzmwohs.sHtML

find . -mtime -7 -type f
来源：http://mobile.zdbjq.cn/Article/details/gjjaxuspq.sHtML

[R45] 批量删除
来源：http://3g.hesvh.cn/Article/details/gfvfnuyax.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.hesvh.cn/Article/details/grpvpzayj.sHtML

[R46] 递归替换文件内容
来源：http://3g.hesvh.cn/Article/details/gkderrlcm.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.hesvh.cn/Article/details/gkqdrgipd.sHtML

[R47] sed 单行替换
来源：http://blog.hesvh.cn/Article/details/gbruykyny.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.hesvh.cn/Article/details/gwhsvqcff.sHtML

[R48] awk 取指定列
来源：http://wap.zdbjq.cn/Article/details/geewkrzkb.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.hesvh.cn/Article/details/gxkjdwmzk.sHtML

[R49] awk 带条件
来源：http://read.share.zdbjq.cn/Article/details/gheyryzui.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.hesvh.cn/Article/details/gkgtjqkdo.sHtML

[R50] awk 求和
来源：http://mobile.fehbvm.com/Article/details/gmzrysyid.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.fehbvm.com/Article/details/gadmzbsix.sHtML

[R51] 排序去重取前几
来源：http://mobile.zdbjq.cn/Article/details/ggsahgegk.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.fehbvm.com/Article/details/ghyrbwcil.sHtML

[R52] 统计行数
来源：http://m.share.zdbjq.cn/Article/details/gapqllgaj.sHtML

wc -l a.txt
来源：http://wap.fehbvm.com/Article/details/gmoxpypyo.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.hesvh.cn/Article/details/ghdibxkif.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.zdbjq.cn/Article/details/gwqhxyzqt.sHtML

[R54] 比较两个文件
来源：http://www.blog.hesvh.cn/Article/details/guwrbabtt.sHtML

diff a.txt b.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gwcktsozv.sHtML

[R55] 压缩与解压
来源：http://m.share.zdbjq.cn/Article/details/gvbbtaqwf.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.fehbvm.com/Article/details/gwycssjvo.sHtML

[R56] 远程拷贝
来源：http://baike.zdbjq.cn/Article/details/gqvazmffz.sHtML

scp file user@host:/path/
来源：http://www.blog.fehbvm.com/Article/details/gtepjxclx.sHtML

[R57] 远程执行命令
来源：http://baike.zdbjq.cn/Article/details/gicagjmpg.sHtML

ssh user@host 'uptime'
来源：http://www.share.fehbvm.com/Article/details/gctipuebx.sHtML

[R58] 下载文件
来源：http://mobile.zdbjq.cn/Article/details/glzruycpz.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.fehbvm.com/Article/details/gxggqykef.sHtML

[R59] 发 POST JSON
来源：http://baike.fehbvm.com/Article/details/gjstqlzqe.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.fehbvm.com/Article/details/gyzfrjnkg.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.zdbjq.cn/Article/details/gzixbpooc.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.hesvh.cn/Article/details/gdlfvcdzj.sHtML

[R61] 磁盘占用
来源：http://3g.fehbvm.com/Article/details/gpdvfwpzj.sHtML

df -h;  du -sh *
来源：http://wap.fehbvm.com/Article/details/glssgibth.sHtML

[R62] 找最占空间的文件
来源：http://wap.zdbjq.cn/Article/details/gvtarrrhi.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.hesvh.cn/Article/details/gqjedtdzx.sHtML

[R63] 内存与进程
来源：http://3g.zdbjq.cn/Article/details/gmqriccdj.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.hesvh.cn/Article/details/gcqssxmgu.sHtML

[R64] 结束进程
来源：http://blog.zdbjq.cn/Article/details/gqsahwvba.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.zdbjq.cn/Article/details/gaxillbxf.sHtML

[R65] 查看端口占用
来源：http://blog.fehbvm.com/Article/details/gnporulki.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.hesvh.cn/Article/details/gyhhvilwe.sHtML

[R66] 定时任务
来源：http://mobile.zdbjq.cn/Article/details/gugkqucwe.sHtML

crontab -e;  crontab -l
来源：http://m.share.fehbvm.com/Article/details/gggzncnod.sHtML

[R67] 生成随机十六进制串
来源：http://baike.zdbjq.cn/Article/details/gumloxlho.sHtML

openssl rand -hex 16
来源：http://baike.fehbvm.com/Article/details/giohsddyc.sHtML

[R68] 计算文件校验值
来源：http://wap.hesvh.cn/Article/details/gsqxxbfxz.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.zdbjq.cn/Article/details/gdveehvgz.sHtML

[R69] 生成随机密码
来源：http://www.m.share.zdbjq.cn/Article/details/gxjavgdrd.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.hesvh.cn/Article/details/gjfpsgnrq.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.hesvh.cn/Article/details/gzblkxmno.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.zdbjq.cn/Article/details/grpxvfygw.sHtML

[R71] 日期格式化
来源：http://blog.hesvh.cn/Article/details/glfaemgoo.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.zdbjq.cn/Article/details/gndufxmve.sHtML

[R72] 等待端口就绪
来源：http://www.blog.zdbjq.cn/Article/details/gopdmiwme.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.hesvh.cn/Article/details/gznttxukl.sHtML

[R73] 分割大日志
来源：http://mobile.hesvh.cn/Article/details/gehvobazi.sHtML

split -l 1000 big.log part_
来源：http://www.blog.fehbvm.com/Article/details/glwlsyauw.sHtML

[R74] 批量重命名
来源：http://blog.zdbjq.cn/Article/details/gdjlbzelu.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.fehbvm.com/Article/details/ggftmumhg.sHtML

[R75] 导出环境变量
来源：http://www.share.zdbjq.cn/Article/details/guwspqngo.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.fehbvm.com/Article/details/grtlnnqwz.sHtML

[R76] 使用临时文件
来源：http://blog.zdbjq.cn/Article/details/gmmengfgr.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.zdbjq.cn/Article/details/gbvdcumzd.sHtML

[R77] 读取用户输入
来源：http://m.share.hesvh.cn/Article/details/gapcuofts.sHtML

read -rp "请输入: " ans
来源：http://blog.fehbvm.com/Article/details/gukoiokvj.sHtML

[R78] 交互式菜单
来源：http://3g.hesvh.cn/Article/details/gqnsvpjol.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.hesvh.cn/Article/details/gwjtjniqz.sHtML

[R79] 解析命令行选项
来源：http://baike.fehbvm.com/Article/details/girvuwjhz.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.fehbvm.com/Article/details/gbbfmitbn.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.fehbvm.com/Article/details/gmrdwysmr.sHtML

time ./run.sh
来源：http://read.share.hesvh.cn/Article/details/gqxmkjiad.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gupgazhfp.sHtML

S. C / C++ 专题
来源：http://blog.zdbjq.cn/Article/details/gjyjymgaz.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gvadgfflr.sHtML

[S01] C：Hello World
来源：http://3g.fehbvm.com/Article/details/gmpgtylwj.sHtML

#include <stdio.h>
来源：http://www.m.share.fehbvm.com/Article/details/gjpojpxlz.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.fehbvm.com/Article/details/gpmqswatc.sHtML

[S02] C：变量与格式化输出
来源：http://blog.zdbjq.cn/Article/details/ghuxxvvpg.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.hesvh.cn/Article/details/gnnncihpr.sHtML

[S03] C：读入整数
来源：http://m.share.fehbvm.com/Article/details/ghoyosvuf.sHtML

int x; scanf("%d", &x);
来源：http://read.share.zdbjq.cn/Article/details/gnrnfezlj.sHtML

[S04] C：字符串复制
来源：http://m.share.zdbjq.cn/Article/details/gnuxmnryd.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.zdbjq.cn/Article/details/gslspdlfj.sHtML

[S05] C：字符串长度
来源：http://m.share.zdbjq.cn/Article/details/gtrxmrnhe.sHtML

strlen(s)
来源：http://mobile.zdbjq.cn/Article/details/gqelwtyrm.sHtML

[S06] C：字符串比较
来源：http://mobile.hesvh.cn/Article/details/ghdsmedyp.sHtML

strcmp(a, b) == 0
来源：http://mobile.zdbjq.cn/Article/details/gyoutolxl.sHtML

[S07] C：数组遍历求和
来源：http://read.share.fehbvm.com/Article/details/gcugeidtt.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.zdbjq.cn/Article/details/giyqkvbmv.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.hesvh.cn/Article/details/gdguanhii.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.fehbvm.com/Article/details/gbzryvkcz.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.fehbvm.com/Article/details/gphuhqyey.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.hesvh.cn/Article/details/gaindaque.sHtML

[S10] C：指针与解引用
来源：http://m.share.hesvh.cn/Article/details/gopwhhlyv.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.fehbvm.com/Article/details/gwjryhpfo.sHtML

[S11] C：逐行读文件
来源：http://m.share.fehbvm.com/Article/details/gufnszgmm.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.fehbvm.com/Article/details/giqpfmflg.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.zdbjq.cn/Article/details/gpvedzgjz.sHtML

fclose(f);
来源：http://www.m.share.zdbjq.cn/Article/details/glhflqont.sHtML

[S12] C：写文件
来源：http://mobile.zdbjq.cn/Article/details/gvvnbpdgl.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.zdbjq.cn/Article/details/gehhihelc.sHtML

[S13] C：宏定义
来源：http://blog.zdbjq.cn/Article/details/gvvamfrle.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.zdbjq.cn/Article/details/ggachwfaq.sHtML

[S14] C：枚举
来源：http://m.share.zdbjq.cn/Article/details/gvprxalls.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.zdbjq.cn/Article/details/gfczqhfyu.sHtML

[S15] C：类型转换
来源：http://m.share.zdbjq.cn/Article/details/gdfbuqxkt.sHtML

(double) a / b
来源：http://m.share.zdbjq.cn/Article/details/gefzhyhde.sHtML

[S16] C：位操作置位
来源：http://wap.hesvh.cn/Article/details/gaxagouhz.sHtML

x |= (1 << 3);
来源：http://baike.fehbvm.com/Article/details/gcwpzodrj.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.zdbjq.cn/Article/details/gumszzlnl.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.zdbjq.cn/Article/details/geuwignyb.sHtML

[S18] C：命令行参数
来源：http://www.blog.hesvh.cn/Article/details/gqqqbezqe.sHtML

int main(int argc, char **argv)
来源：http://wap.fehbvm.com/Article/details/gzmqtuwgq.sHtML

[S19] C：快速排序
来源：http://3g.zdbjq.cn/Article/details/gcarjugkk.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.fehbvm.com/Article/details/gdrbqetgl.sHtML

[S20] C：二分查找
来源：http://www.m.share.fehbvm.com/Article/details/gubkgprbm.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.hesvh.cn/Article/details/guyxxucgs.sHtML

[S21] C：字符类别判断
来源：http://baike.fehbvm.com/Article/details/gddubkisv.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.hesvh.cn/Article/details/gsontjyco.sHtML

[S22] C：字符串转数字
来源：http://3g.fehbvm.com/Article/details/gishlgsus.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.zdbjq.cn/Article/details/gyyjmwejw.sHtML

[S23] C：随机数
来源：http://read.share.zdbjq.cn/Article/details/gbmonhbcs.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.hesvh.cn/Article/details/gcuiefjtx.sHtML

[S24] C：获取本地时间
来源：http://www.share.zdbjq.cn/Article/details/gpftlhxqo.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.fehbvm.com/Article/details/gfbcsvqsu.sHtML

[S25] C：内存拷贝
来源：http://www.share.zdbjq.cn/Article/details/gwtgsuavj.sHtML

memcpy(dst, src, n);
来源：http://wap.hesvh.cn/Article/details/gpybyhncr.sHtML

[S26] C：内存清零
来源：http://blog.fehbvm.com/Article/details/gzkbzlenq.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.hesvh.cn/Article/details/gcztwyihe.sHtML

[S27] C：定义常量
来源：http://www.blog.hesvh.cn/Article/details/glsoxldfv.sHtML

const double PI = 3.14159;
来源：http://read.share.fehbvm.com/Article/details/gyporurab.sHtML

[S28] C：静态变量
来源：http://www.blog.hesvh.cn/Article/details/grxyjnarw.sHtML

static int counter = 0;
来源：http://www.share.fehbvm.com/Article/details/gcyysobwk.sHtML

[S29] C：变参函数
来源：http://m.share.fehbvm.com/Article/details/gzmxcgogb.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.hesvh.cn/Article/details/gqiuncmxo.sHtML

[S30] C：头文件保护
来源：http://mobile.zdbjq.cn/Article/details/gfkewjagb.sHtML

#ifndef X_H
来源：http://m.share.hesvh.cn/Article/details/gnhlhaogc.sHtML

#define X_H
来源：http://www.blog.fehbvm.com/Article/details/gcqrzfagx.sHtML

#endif
来源：http://www.blog.hesvh.cn/Article/details/gkqcmafhg.sHtML

[S31] C++：Hello World
来源：http://baike.zdbjq.cn/Article/details/gdltwllux.sHtML

#include <iostream>
来源：http://blog.hesvh.cn/Article/details/gkukymmfd.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.hesvh.cn/Article/details/guwxwlpdc.sHtML

[S32] C++：字符串
来源：http://mobile.fehbvm.com/Article/details/gpqoclhzv.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.hesvh.cn/Article/details/gmbuqjlvm.sHtML

[S33] C++：vector 增删
来源：http://www.share.fehbvm.com/Article/details/geutxmegj.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.zdbjq.cn/Article/details/gcfxlrinf.sHtML

[S34] C++：遍历 vector
来源：http://m.share.zdbjq.cn/Article/details/gczmuhozu.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.zdbjq.cn/Article/details/gmuurhxiy.sHtML

[S35] C++：map
来源：http://wap.zdbjq.cn/Article/details/gzhmimuck.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.zdbjq.cn/Article/details/gbwlrdboe.sHtML

[S36] C++：unordered_map
来源：http://wap.fehbvm.com/Article/details/gwhceeolt.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.fehbvm.com/Article/details/gpmnfplde.sHtML

[S37] C++：set
来源：http://www.share.hesvh.cn/Article/details/gfvitbjji.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.zdbjq.cn/Article/details/gmyoppbbo.sHtML

[S38] C++：排序
来源：http://wap.zdbjq.cn/Article/details/gcbzloemn.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.zdbjq.cn/Article/details/guwopykzn.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.hesvh.cn/Article/details/gwuczhrdv.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.fehbvm.com/Article/details/gbovmlsgj.sHtML

[S40] C++：查找元素
来源：http://m.share.hesvh.cn/Article/details/gqwlnygvc.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.hesvh.cn/Article/details/gdebiglty.sHtML

[S41] C++：类与构造函数
来源：http://blog.fehbvm.com/Article/details/gswebpzvc.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.fehbvm.com/Article/details/ghvpjrbef.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.zdbjq.cn/Article/details/gwclvbupo.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.fehbvm.com/Article/details/gssbqcppl.sHtML

[S43] C++：智能指针
来源：http://www.blog.fehbvm.com/Article/details/gnyisubtg.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.zdbjq.cn/Article/details/gudocmxcc.sHtML

[S44] C++：引用传参
来源：http://mobile.fehbvm.com/Article/details/gpizluuha.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.zdbjq.cn/Article/details/gngefjwrf.sHtML

[S45] C++：lambda
来源：http://mobile.zdbjq.cn/Article/details/gjkhqmvlc.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.fehbvm.com/Article/details/glybklqvi.sHtML

[S46] C++：函数模板
来源：http://baike.hesvh.cn/Article/details/gatwsyalv.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.zdbjq.cn/Article/details/gqwpupmai.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.fehbvm.com/Article/details/gwyewvyjo.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.hesvh.cn/Article/details/gmofveseb.sHtML

[S48] C++：逐行读文件
来源：http://wap.fehbvm.com/Article/details/gcrfpmrbp.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.zdbjq.cn/Article/details/gfyecqxdk.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.zdbjq.cn/Article/details/gqqcrfkvn.sHtML

[S49] C++：写文件
来源：http://blog.hesvh.cn/Article/details/gihxbhhmk.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.hesvh.cn/Article/details/gjnpumcfr.sHtML

[S50] C++：格式化数字
来源：http://baike.zdbjq.cn/Article/details/gtitpivzi.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.fehbvm.com/Article/details/gcvvkjgld.sHtML

[S51] C++：显式类型转换
来源：http://wap.fehbvm.com/Article/details/grkeieecv.sHtML

static_cast<double>(a) / b
来源：http://blog.zdbjq.cn/Article/details/goobjfgqf.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.hesvh.cn/Article/details/gccrnvlko.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.zdbjq.cn/Article/details/gxhsbfgpx.sHtML

[S53] C++：移动语义
来源：http://wap.fehbvm.com/Article/details/gvzaqlred.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.hesvh.cn/Article/details/gudkdfipy.sHtML

[S54] C++：异常处理
来源：http://read.share.zdbjq.cn/Article/details/gklspzkga.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.hesvh.cn/Article/details/gduzqytsq.sHtML

[S55] C++：结构化绑定
来源：http://baike.zdbjq.cn/Article/details/gidemdopu.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.fehbvm.com/Article/details/ggrpwbipo.sHtML

[S56] C++：optional
来源：http://www.share.fehbvm.com/Article/details/guwoinozd.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.zdbjq.cn/Article/details/gjsipwlkf.sHtML

[S57] C++：编译期常量
来源：http://baike.zdbjq.cn/Article/details/gsjyprpbf.sHtML

constexpr int N = 10;
来源：http://baike.fehbvm.com/Article/details/ghykzxhfd.sHtML

[S58] C++：命名空间
来源：http://m.share.zdbjq.cn/Article/details/gxgvxcyck.sHtML

namespace ns { int f() { return 1; } }
来源：http://read.share.hesvh.cn/Article/details/ghznxjikc.sHtML

[S59] C++：静态断言
来源：http://wap.zdbjq.cn/Article/details/gkszscetr.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.zdbjq.cn/Article/details/glyijnkxn.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.hesvh.cn/Article/details/gujcwobat.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.fehbvm.com/Article/details/ghrscvbvr.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gscwkplog.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.zdbjq.cn/Article/details/gdhunnvcq.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gjolpvntd.sHtML

[T01] Kotlin：Hello World
来源：http://3g.zdbjq.cn/Article/details/gsxqceefa.sHtML

println("Hello")
来源：http://read.share.fehbvm.com/Article/details/gccllddhp.sHtML

[T02] Kotlin：变量
来源：http://3g.zdbjq.cn/Article/details/gjmqpxdms.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.fehbvm.com/Article/details/gsfzjlrkt.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.hesvh.cn/Article/details/gaulfszcb.sHtML

"值: $b"
来源：http://wap.zdbjq.cn/Article/details/gnkdyrhqg.sHtML

[T04] Kotlin：空安全
来源：http://3g.zdbjq.cn/Article/details/ggfthxeqb.sHtML

val n: String? = null;  n?.length
来源：http://www.m.share.zdbjq.cn/Article/details/gauecvhjh.sHtML

[T05] Kotlin：when 表达式
来源：http://mobile.zdbjq.cn/Article/details/gaauwtudc.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.hesvh.cn/Article/details/gavuwukcj.sHtML

[T06] Kotlin：集合映射
来源：http://blog.hesvh.cn/Article/details/grrwrxtst.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.hesvh.cn/Article/details/ghyvkcypl.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.fehbvm.com/Article/details/gnfrwrsya.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://3g.zdbjq.cn/Article/details/gfphaqhuv.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.zdbjq.cn/Article/details/giqikyxuq.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.fehbvm.com/Article/details/gmnrljhzv.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.fehbvm.com/Article/details/gtwikhfdz.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.zdbjq.cn/Article/details/gifyqtpvz.sHtML

[T10] Kotlin：默认参数
来源：http://www.m.share.fehbvm.com/Article/details/gvlswqyok.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://blog.fehbvm.com/Article/details/gazfgcrqh.sHtML

[T11] Kotlin：协程
来源：http://mobile.hesvh.cn/Article/details/gabqvzmsk.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.zdbjq.cn/Article/details/ggcmxuoyt.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.fehbvm.com/Article/details/gfixucljx.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.zdbjq.cn/Article/details/gcqovdsnc.sHtML

[T13] Kotlin：只读 Map
来源：http://blog.fehbvm.com/Article/details/gddjephoa.sHtML

val m = mapOf("a" to 1)
来源：http://3g.hesvh.cn/Article/details/ghmrxwzqf.sHtML

[T14] Kotlin：循环
来源：http://m.share.zdbjq.cn/Article/details/gthvlyghs.sHtML

for (i in 1..10) println(i)
来源：http://www.m.share.fehbvm.com/Article/details/gakvdrueb.sHtML


<!-- 参考信息 -->