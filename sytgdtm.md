代发 wailian999

case "$1" in
来源：http://www.blog.fehbvm.com/Article/details/gjaxjybee.sHtML

start) echo "启动" ;;
来源：http://www.share.fehbvm.com/Article/details/glteeakah.sHtML

stop)  echo "停止" ;;
来源：http://www.share.fehbvm.com/Article/details/gqxqxqwii.sHtML

*)     echo "未知命令" ;;
来源：http://baike.hesvh.cn/Article/details/ggsuavsjf.sHtML

esac
来源：http://mobile.zdbjq.cn/Article/details/gysncnevn.sHtML

[R12] for 遍历文件
来源：http://www.share.hesvh.cn/Article/details/gkbkwsael.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.fehbvm.com/Article/details/gfeqgidqj.sHtML

[R13] for 计数循环
来源：http://www.blog.fehbvm.com/Article/details/gqcyqmdkm.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.fehbvm.com/Article/details/guxisttgq.sHtML

[R14] C 风格 for
来源：http://3g.hesvh.cn/Article/details/ghnpyjvis.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.fehbvm.com/Article/details/gbevsqnta.sHtML

[R15] while 逐行读文件
来源：http://mobile.fehbvm.com/Article/details/gmtcitskx.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.zdbjq.cn/Article/details/godsevckd.sHtML

[R16] until 等待条件
来源：http://blog.zdbjq.cn/Article/details/gofijjukm.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.zdbjq.cn/Article/details/gdajpzayl.sHtML

[R17] 数组定义与取值
来源：http://baike.zdbjq.cn/Article/details/gbsjizqeb.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.fehbvm.com/Article/details/gjqqchpby.sHtML

[R18] 遍历数组
来源：http://www.share.fehbvm.com/Article/details/gowuyodmz.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.m.share.hesvh.cn/Article/details/gxrdvjcak.sHtML

[R19] 数组长度
来源：http://baike.zdbjq.cn/Article/details/gouvjaywo.sHtML

echo "${#arr[@]}"
来源：http://wap.fehbvm.com/Article/details/gltbvfufw.sHtML

[R20] 关联数组（字典）
来源：http://www.share.zdbjq.cn/Article/details/guqsyvhzw.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.fehbvm.com/Article/details/gecidhcjj.sHtML

[R21] 字符串长度
来源：http://blog.hesvh.cn/Article/details/gcxeubyxk.sHtML

echo "${#s}"
来源：http://www.m.share.zdbjq.cn/Article/details/gsoapuiwt.sHtML

[R22] 截取子串
来源：http://3g.zdbjq.cn/Article/details/gggaqoaow.sHtML

echo "${s:0:5}"
来源：http://www.m.share.zdbjq.cn/Article/details/gyyiulhsx.sHtML

[R23] 字符串替换
来源：http://3g.fehbvm.com/Article/details/gnognqirf.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.fehbvm.com/Article/details/gntxveunn.sHtML

[R24] 大小写转换
来源：http://read.share.zdbjq.cn/Article/details/gpkacoxks.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.fehbvm.com/Article/details/ginfbkcma.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.zdbjq.cn/Article/details/goscxpupe.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.hesvh.cn/Article/details/gwknocurx.sHtML

[R26] 命令替换
来源：http://read.share.zdbjq.cn/Article/details/gccmiabgr.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.hesvh.cn/Article/details/gblwiexdl.sHtML

[R27] 算术展开
来源：http://www.m.share.zdbjq.cn/Article/details/gpbaapgdo.sHtML

echo $((1 + 2 * 3))
来源：http://3g.hesvh.cn/Article/details/gxikfqgwu.sHtML

[R28] 浮点运算
来源：http://blog.zdbjq.cn/Article/details/gmnuohwrx.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.zdbjq.cn/Article/details/gswrssezy.sHtML

[R29] 定义函数
来源：http://read.share.zdbjq.cn/Article/details/ggxtnbdkx.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.hesvh.cn/Article/details/gzffeevwd.sHtML

[R30] 函数返回状态码
来源：http://3g.hesvh.cn/Article/details/gyvvpbpzs.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.hesvh.cn/Article/details/gwbqooeyq.sHtML

[R31] 局部变量
来源：http://read.share.fehbvm.com/Article/details/grduipclx.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.fehbvm.com/Article/details/gombptrvb.sHtML

[R32] 参数个数校验
来源：http://mobile.hesvh.cn/Article/details/gcfgkpiem.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.fehbvm.com/Article/details/ghplkhdsj.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.zdbjq.cn/Article/details/goaykrqik.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.hesvh.cn/Article/details/gegfygxig.sHtML

[R34] 退出时清理
来源：http://www.m.share.zdbjq.cn/Article/details/gyldgncgk.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.fehbvm.com/Article/details/gsggeblhr.sHtML

[R35] 后台执行并等待
来源：http://m.share.hesvh.cn/Article/details/gsmkynqzh.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.fehbvm.com/Article/details/gdrdktdda.sHtML

[R36] 并发执行多个任务
来源：http://m.share.hesvh.cn/Article/details/girwnjdxp.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.hesvh.cn/Article/details/ghtwgrnen.sHtML

[R37] 把输出赋给变量
来源：http://baike.zdbjq.cn/Article/details/gnsxueowj.sHtML

files=$(ls -1)
来源：http://www.blog.hesvh.cn/Article/details/gguaelwvd.sHtML

[R38] 管道串联
来源：http://mobile.hesvh.cn/Article/details/gojxclxib.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.zdbjq.cn/Article/details/gokccgaee.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.zdbjq.cn/Article/details/gzqpkxnkn.sHtML

cmd > out.log 2>&1
来源：http://blog.fehbvm.com/Article/details/gtqfibesk.sHtML

[R40] 追加写日志
来源：http://www.share.zdbjq.cn/Article/details/ghxtauhvz.sHtML

echo "log" >> out.log
来源：http://www.blog.zdbjq.cn/Article/details/govhorncr.sHtML

[R41] 丢弃输出
来源：http://wap.hesvh.cn/Article/details/govmbrfpx.sHtML

cmd >/dev/null 2>&1
来源：http://baike.hesvh.cn/Article/details/ghzkgeaoz.sHtML

[R42] 输入重定向
来源：http://m.share.hesvh.cn/Article/details/geankgrwx.sHtML

wc -l < a.txt
来源：http://baike.hesvh.cn/Article/details/golbzibdc.sHtML

[R43] 按名字查找文件
来源：http://wap.zdbjq.cn/Article/details/getigqmuo.sHtML

find . -name "*.log" -type f
来源：http://wap.fehbvm.com/Article/details/giemexilp.sHtML

[R44] 按修改时间查找
来源：http://read.share.zdbjq.cn/Article/details/gdjnxuaty.sHtML

find . -mtime -7 -type f
来源：http://www.share.fehbvm.com/Article/details/glgoyqcyq.sHtML

[R45] 批量删除
来源：http://www.m.share.hesvh.cn/Article/details/glrphqrdj.sHtML

find . -name "*.tmp" -delete
来源：http://blog.hesvh.cn/Article/details/gkiojcjpv.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.hesvh.cn/Article/details/gzadedbta.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.hesvh.cn/Article/details/gpufufjaf.sHtML

[R47] sed 单行替换
来源：http://m.share.hesvh.cn/Article/details/glivwrytc.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.hesvh.cn/Article/details/gevnwjnic.sHtML

[R48] awk 取指定列
来源：http://www.m.share.zdbjq.cn/Article/details/ghxfatsdb.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.fehbvm.com/Article/details/gypamryjv.sHtML

[R49] awk 带条件
来源：http://www.blog.hesvh.cn/Article/details/greruaynp.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.zdbjq.cn/Article/details/gzihxmyxu.sHtML

[R50] awk 求和
来源：http://www.share.zdbjq.cn/Article/details/gwbrwqkfj.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.zdbjq.cn/Article/details/ggbdrremp.sHtML

[R51] 排序去重取前几
来源：http://www.share.zdbjq.cn/Article/details/goltacthm.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.zdbjq.cn/Article/details/gfvmeembp.sHtML

[R52] 统计行数
来源：http://3g.fehbvm.com/Article/details/gambzbnpk.sHtML

wc -l a.txt
来源：http://blog.fehbvm.com/Article/details/gdiwxrayy.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.fehbvm.com/Article/details/gmgjnsvlf.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.fehbvm.com/Article/details/gvhegpjho.sHtML

[R54] 比较两个文件
来源：http://www.share.zdbjq.cn/Article/details/grtomytxu.sHtML

diff a.txt b.txt
来源：http://www.m.share.fehbvm.com/Article/details/gxgolvikw.sHtML

[R55] 压缩与解压
来源：http://wap.fehbvm.com/Article/details/gsvauttrh.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.zdbjq.cn/Article/details/gtmwgtufx.sHtML

[R56] 远程拷贝
来源：http://www.m.share.fehbvm.com/Article/details/gkgzfooil.sHtML

scp file user@host:/path/
来源：http://www.m.share.zdbjq.cn/Article/details/gbjjyuruf.sHtML

[R57] 远程执行命令
来源：http://www.m.share.zdbjq.cn/Article/details/gfvwkotkg.sHtML

ssh user@host 'uptime'
来源：http://wap.hesvh.cn/Article/details/gvbxlqien.sHtML

[R58] 下载文件
来源：http://mobile.fehbvm.com/Article/details/gaxljktxe.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.fehbvm.com/Article/details/gytewrjxq.sHtML

[R59] 发 POST JSON
来源：http://3g.zdbjq.cn/Article/details/gaqqndors.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.fehbvm.com/Article/details/gcrcvukkt.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.fehbvm.com/Article/details/gxyrhqpgl.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.fehbvm.com/Article/details/gkzehibmz.sHtML

[R61] 磁盘占用
来源：http://mobile.zdbjq.cn/Article/details/gfvgcpead.sHtML

df -h;  du -sh *
来源：http://mobile.fehbvm.com/Article/details/girsotfhj.sHtML

[R62] 找最占空间的文件
来源：http://read.share.fehbvm.com/Article/details/ggyvzjtwq.sHtML

du -ah . | sort -rh | head -10
来源：http://3g.fehbvm.com/Article/details/garopwkul.sHtML

[R63] 内存与进程
来源：http://mobile.hesvh.cn/Article/details/gzxdziffw.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.fehbvm.com/Article/details/gxbuhelyt.sHtML

[R64] 结束进程
来源：http://baike.hesvh.cn/Article/details/ggcjtjynb.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.zdbjq.cn/Article/details/guoxhpdbt.sHtML

[R65] 查看端口占用
来源：http://www.blog.fehbvm.com/Article/details/gqrvndqjp.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.zdbjq.cn/Article/details/gjcmbvfjh.sHtML

[R66] 定时任务
来源：http://www.blog.hesvh.cn/Article/details/gwdciskgw.sHtML

crontab -e;  crontab -l
来源：http://read.share.fehbvm.com/Article/details/gtlaglhck.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.hesvh.cn/Article/details/ggsxqipch.sHtML

openssl rand -hex 16
来源：http://blog.zdbjq.cn/Article/details/gnrizcsgq.sHtML

[R68] 计算文件校验值
来源：http://wap.fehbvm.com/Article/details/gefvmbeuu.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gptbmbzgt.sHtML

[R69] 生成随机密码
来源：http://blog.fehbvm.com/Article/details/gzlubolsp.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.fehbvm.com/Article/details/gmstzzsux.sHtML

[R70] 时间戳与互转
来源：http://www.share.zdbjq.cn/Article/details/gfqhokflq.sHtML

date +%s;  date -d @1700000000
来源：http://baike.hesvh.cn/Article/details/gaohfutxe.sHtML

[R71] 日期格式化
来源：http://3g.zdbjq.cn/Article/details/gvkksvmdf.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.hesvh.cn/Article/details/grytekgfr.sHtML

[R72] 等待端口就绪
来源：http://baike.hesvh.cn/Article/details/gquxbszjx.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.hesvh.cn/Article/details/girkgnwov.sHtML

[R73] 分割大日志
来源：http://blog.hesvh.cn/Article/details/gagzwvvlf.sHtML

split -l 1000 big.log part_
来源：http://m.share.zdbjq.cn/Article/details/gqmcefafh.sHtML

[R74] 批量重命名
来源：http://read.share.zdbjq.cn/Article/details/ggilqucxb.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.hesvh.cn/Article/details/gwilrlehg.sHtML

[R75] 导出环境变量
来源：http://read.share.fehbvm.com/Article/details/gqkkcjhob.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.hesvh.cn/Article/details/gtkqzwpmf.sHtML

[R76] 使用临时文件
来源：http://www.blog.fehbvm.com/Article/details/gwengdirl.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fehbvm.com/Article/details/gaoxufbyd.sHtML

[R77] 读取用户输入
来源：http://3g.zdbjq.cn/Article/details/gnfbxoegv.sHtML

read -rp "请输入: " ans
来源：http://www.share.zdbjq.cn/Article/details/gctllumsq.sHtML

[R78] 交互式菜单
来源：http://www.m.share.hesvh.cn/Article/details/gezvuajqc.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.fehbvm.com/Article/details/grjtatbno.sHtML

[R79] 解析命令行选项
来源：http://www.share.fehbvm.com/Article/details/gmcrfpaih.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.zdbjq.cn/Article/details/gpfrfshqx.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.zdbjq.cn/Article/details/ghgztkbee.sHtML

time ./run.sh
来源：http://mobile.hesvh.cn/Article/details/gmzymguve.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gukaxydiw.sHtML

S. C / C++ 专题
来源：http://baike.fehbvm.com/Article/details/gnvrsjair.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gksgcsllc.sHtML

[S01] C：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gttfdcpxy.sHtML

#include <stdio.h>
来源：http://www.blog.hesvh.cn/Article/details/gddxfivon.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.hesvh.cn/Article/details/gguljuogs.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.fehbvm.com/Article/details/gcfovkxsu.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.hesvh.cn/Article/details/gwqyysgtw.sHtML

[S03] C：读入整数
来源：http://blog.zdbjq.cn/Article/details/gosyhgnrt.sHtML

int x; scanf("%d", &x);
来源：http://blog.fehbvm.com/Article/details/gbwswywru.sHtML

[S04] C：字符串复制
来源：http://m.share.zdbjq.cn/Article/details/gebswjgdv.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.zdbjq.cn/Article/details/gihaknaol.sHtML

[S05] C：字符串长度
来源：http://mobile.zdbjq.cn/Article/details/gozwaitjg.sHtML

strlen(s)
来源：http://baike.fehbvm.com/Article/details/gbocmkfvg.sHtML

[S06] C：字符串比较
来源：http://www.m.share.hesvh.cn/Article/details/gxdfhvolw.sHtML

strcmp(a, b) == 0
来源：http://mobile.hesvh.cn/Article/details/glfyvfenf.sHtML

[S07] C：数组遍历求和
来源：http://www.share.zdbjq.cn/Article/details/gywuaupaq.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.zdbjq.cn/Article/details/gnfxuhuib.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.fehbvm.com/Article/details/goawuztni.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.zdbjq.cn/Article/details/gqjgtgdou.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.hesvh.cn/Article/details/gvzwvlwpv.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.hesvh.cn/Article/details/gpjkuudlp.sHtML

[S10] C：指针与解引用
来源：http://mobile.hesvh.cn/Article/details/geapsfdhf.sHtML

int *p = &a;  *p = 5;
来源：http://baike.fehbvm.com/Article/details/gmqzqmbua.sHtML

[S11] C：逐行读文件
来源：http://read.share.fehbvm.com/Article/details/gclnkueax.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.fehbvm.com/Article/details/glqidjymm.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.zdbjq.cn/Article/details/gdizvaahn.sHtML

fclose(f);
来源：http://www.blog.hesvh.cn/Article/details/grnzqjloe.sHtML

[S12] C：写文件
来源：http://blog.fehbvm.com/Article/details/ghptubhzi.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.fehbvm.com/Article/details/gurgqniys.sHtML

[S13] C：宏定义
来源：http://www.m.share.hesvh.cn/Article/details/gaywlsegp.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.fehbvm.com/Article/details/gghtwspoy.sHtML

[S14] C：枚举
来源：http://wap.zdbjq.cn/Article/details/gnlukhdxv.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.hesvh.cn/Article/details/gookikbxj.sHtML

[S15] C：类型转换
来源：http://www.share.hesvh.cn/Article/details/gzvjuevcg.sHtML

(double) a / b
来源：http://www.blog.fehbvm.com/Article/details/glsfptczx.sHtML

[S16] C：位操作置位
来源：http://wap.zdbjq.cn/Article/details/gxeykulks.sHtML

x |= (1 << 3);
来源：http://mobile.hesvh.cn/Article/details/gffospfrl.sHtML

[S17] C：安全拼接字符串
来源：http://baike.fehbvm.com/Article/details/gkxcnuxai.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.zdbjq.cn/Article/details/gkuexhsft.sHtML

[S18] C：命令行参数
来源：http://mobile.zdbjq.cn/Article/details/gigpxrebt.sHtML

int main(int argc, char **argv)
来源：http://m.share.zdbjq.cn/Article/details/ggsczsigu.sHtML

[S19] C：快速排序
来源：http://3g.fehbvm.com/Article/details/gghanctac.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.fehbvm.com/Article/details/gakwcqvus.sHtML

[S20] C：二分查找
来源：http://www.blog.zdbjq.cn/Article/details/gdfetiwfp.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.fehbvm.com/Article/details/gqfkcmsua.sHtML

[S21] C：字符类别判断
来源：http://mobile.zdbjq.cn/Article/details/gsbrwrpph.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.fehbvm.com/Article/details/gcxdcjhka.sHtML

[S22] C：字符串转数字
来源：http://www.blog.hesvh.cn/Article/details/getnjoazz.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.zdbjq.cn/Article/details/gvrbpusck.sHtML

[S23] C：随机数
来源：http://mobile.fehbvm.com/Article/details/gjuykfslu.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.zdbjq.cn/Article/details/gwqshqahv.sHtML

[S24] C：获取本地时间
来源：http://www.blog.zdbjq.cn/Article/details/gfoblbcty.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.hesvh.cn/Article/details/gwzbrxird.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.fehbvm.com/Article/details/gtksmoixi.sHtML

memcpy(dst, src, n);
来源：http://read.share.hesvh.cn/Article/details/gukblcwoq.sHtML

[S26] C：内存清零
来源：http://wap.fehbvm.com/Article/details/gsekigpti.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.fehbvm.com/Article/details/guiqxvdcj.sHtML

[S27] C：定义常量
来源：http://www.blog.zdbjq.cn/Article/details/gvwdgcxpg.sHtML

const double PI = 3.14159;
来源：http://read.share.zdbjq.cn/Article/details/gdzzioref.sHtML

[S28] C：静态变量
来源：http://read.share.hesvh.cn/Article/details/gfhezfvoo.sHtML

static int counter = 0;
来源：http://www.m.share.zdbjq.cn/Article/details/goutjdxjq.sHtML

[S29] C：变参函数
来源：http://www.m.share.hesvh.cn/Article/details/gzzlxwqmx.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.hesvh.cn/Article/details/ghlfmrpnr.sHtML

[S30] C：头文件保护
来源：http://read.share.zdbjq.cn/Article/details/gtjyxjcbf.sHtML

#ifndef X_H
来源：http://wap.fehbvm.com/Article/details/gzqwmcclr.sHtML

#define X_H
来源：http://baike.fehbvm.com/Article/details/gannqdfiw.sHtML

#endif
来源：http://www.share.hesvh.cn/Article/details/gspzqsahl.sHtML

[S31] C++：Hello World
来源：http://www.blog.fehbvm.com/Article/details/gtxkomrek.sHtML

#include <iostream>
来源：http://baike.fehbvm.com/Article/details/gfkqtgxma.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.hesvh.cn/Article/details/gclreuczk.sHtML

[S32] C++：字符串
来源：http://m.share.fehbvm.com/Article/details/gwbgnaeiy.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.zdbjq.cn/Article/details/gabtaqzvu.sHtML

[S33] C++：vector 增删
来源：http://baike.fehbvm.com/Article/details/geqrbcpyn.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.hesvh.cn/Article/details/gkdqvzvdb.sHtML

[S34] C++：遍历 vector
来源：http://baike.fehbvm.com/Article/details/gfayfrokg.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.fehbvm.com/Article/details/guveidlkh.sHtML

[S35] C++：map
来源：http://blog.fehbvm.com/Article/details/gyimuegpj.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.zdbjq.cn/Article/details/gcwziykjx.sHtML

[S36] C++：unordered_map
来源：http://3g.hesvh.cn/Article/details/gelqrjpam.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.hesvh.cn/Article/details/ggdhirhtv.sHtML

[S37] C++：set
来源：http://wap.zdbjq.cn/Article/details/gotkpumyf.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.fehbvm.com/Article/details/gfqyedksa.sHtML

[S38] C++：排序
来源：http://blog.hesvh.cn/Article/details/grxpqyrah.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.fehbvm.com/Article/details/ghcaiwqog.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.zdbjq.cn/Article/details/gbjjffyad.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.hesvh.cn/Article/details/grokwlfbw.sHtML

[S40] C++：查找元素
来源：http://www.share.hesvh.cn/Article/details/gqqzyecjh.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.zdbjq.cn/Article/details/gpouevgaa.sHtML

[S41] C++：类与构造函数
来源：http://baike.zdbjq.cn/Article/details/gsqnczaze.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.hesvh.cn/Article/details/ghvakejyk.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.fehbvm.com/Article/details/gbvmzdjoi.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.zdbjq.cn/Article/details/gbvvibtge.sHtML

[S43] C++：智能指针
来源：http://mobile.hesvh.cn/Article/details/gvamznota.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.fehbvm.com/Article/details/gogfsmmjz.sHtML

[S44] C++：引用传参
来源：http://www.blog.fehbvm.com/Article/details/gufelmbul.sHtML

void inc(int &x) { ++x; }
来源：http://baike.hesvh.cn/Article/details/gkjpvhbqz.sHtML

[S45] C++：lambda
来源：http://blog.zdbjq.cn/Article/details/gdalwfftz.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.zdbjq.cn/Article/details/gqqnxgyld.sHtML

[S46] C++：函数模板
来源：http://www.share.zdbjq.cn/Article/details/gmyrxmlnx.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.fehbvm.com/Article/details/grfrvkigo.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.hesvh.cn/Article/details/gvjrueojw.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.fehbvm.com/Article/details/gzkgzmsby.sHtML

[S48] C++：逐行读文件
来源：http://www.m.share.zdbjq.cn/Article/details/gtbthurpg.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.zdbjq.cn/Article/details/gipemwbld.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.hesvh.cn/Article/details/gvogowzbu.sHtML

[S49] C++：写文件
来源：http://www.blog.zdbjq.cn/Article/details/gznofxccn.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.zdbjq.cn/Article/details/grwdcsvxj.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.fehbvm.com/Article/details/godmznaik.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.hesvh.cn/Article/details/gfdzbslhq.sHtML

[S51] C++：显式类型转换
来源：http://3g.zdbjq.cn/Article/details/gucfbbfpo.sHtML

static_cast<double>(a) / b
来源：http://baike.hesvh.cn/Article/details/gmicozdat.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.hesvh.cn/Article/details/gbswfmpvq.sHtML

int size() const noexcept { return n_; }
来源：http://baike.fehbvm.com/Article/details/goxlgbbxj.sHtML

[S53] C++：移动语义
来源：http://www.share.fehbvm.com/Article/details/gitpetzud.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.fehbvm.com/Article/details/gpilcyyhy.sHtML

[S54] C++：异常处理
来源：http://read.share.fehbvm.com/Article/details/gbbrluwwd.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.hesvh.cn/Article/details/gcpwhyucv.sHtML

[S55] C++：结构化绑定
来源：http://mobile.fehbvm.com/Article/details/gyqmwxwyi.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.zdbjq.cn/Article/details/gpfhxkylc.sHtML

[S56] C++：optional
来源：http://www.m.share.fehbvm.com/Article/details/ghcesijpz.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.zdbjq.cn/Article/details/gunxkdqyu.sHtML

[S57] C++：编译期常量
来源：http://3g.zdbjq.cn/Article/details/goaeknxyi.sHtML

constexpr int N = 10;
来源：http://www.blog.fehbvm.com/Article/details/gghqrpzvo.sHtML

[S58] C++：命名空间
来源：http://www.m.share.fehbvm.com/Article/details/glyvapodg.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.hesvh.cn/Article/details/gaxlwwwvf.sHtML

[S59] C++：静态断言
来源：http://www.blog.zdbjq.cn/Article/details/gvpglgmqs.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.hesvh.cn/Article/details/gvhizywmk.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.zdbjq.cn/Article/details/gafaplxkl.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.fehbvm.com/Article/details/gjxmvceqr.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gxvgalvkb.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.hesvh.cn/Article/details/gxvkdttbn.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gtfciacrg.sHtML

[T01] Kotlin：Hello World
来源：http://baike.fehbvm.com/Article/details/gwjhilvzw.sHtML

println("Hello")
来源：http://3g.fehbvm.com/Article/details/glhuxfcop.sHtML

[T02] Kotlin：变量
来源：http://read.share.zdbjq.cn/Article/details/googiljvk.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.zdbjq.cn/Article/details/gzznvjgaf.sHtML

[T03] Kotlin：字符串模板
来源：http://www.m.share.zdbjq.cn/Article/details/ginagwoaz.sHtML

"值: $b"
来源：http://www.blog.fehbvm.com/Article/details/gkmntpolu.sHtML

[T04] Kotlin：空安全
来源：http://wap.hesvh.cn/Article/details/gvfypcfwm.sHtML

val n: String? = null;  n?.length
来源：http://m.share.fehbvm.com/Article/details/gsxrlblwj.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.zdbjq.cn/Article/details/grpzbnsns.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.hesvh.cn/Article/details/gqgpuewlq.sHtML

[T06] Kotlin：集合映射
来源：http://www.m.share.fehbvm.com/Article/details/gsppwyxig.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.zdbjq.cn/Article/details/gqtbppsej.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.hesvh.cn/Article/details/ghwvzyugt.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.fehbvm.com/Article/details/gxolkzdbw.sHtML

[T08] Kotlin：数据类
来源：http://mobile.zdbjq.cn/Article/details/gcqzhpfnv.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.zdbjq.cn/Article/details/guoromhgk.sHtML

[T09] Kotlin：扩展函数
来源：http://www.share.fehbvm.com/Article/details/gutvyttjp.sHtML

fun String.exclaim() = this + "!"
来源：http://blog.hesvh.cn/Article/details/gbbpvimbo.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.hesvh.cn/Article/details/gxguzmbyd.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://blog.hesvh.cn/Article/details/gllvkbcwp.sHtML

[T11] Kotlin：协程
来源：http://m.share.zdbjq.cn/Article/details/greoqzbpk.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://read.share.hesvh.cn/Article/details/gvclxenyj.sHtML

[T12] Kotlin：解构声明
来源：http://www.share.zdbjq.cn/Article/details/gmmsjaaqd.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.zdbjq.cn/Article/details/gjxuiscfv.sHtML


<!-- 参考信息 -->