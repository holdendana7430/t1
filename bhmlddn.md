代发 wailian999

case "$1" in
来源：http://www.blog.zdbjq.cn/Article/details/gdazllboi.sHtML

start) echo "启动" ;;
来源：http://mobile.hesvh.cn/Article/details/gmujbeyki.sHtML

stop)  echo "停止" ;;
来源：http://www.share.zdbjq.cn/Article/details/gykfpxgiq.sHtML

*)     echo "未知命令" ;;
来源：http://blog.fehbvm.com/Article/details/ghrpxwhex.sHtML

esac
来源：http://www.m.share.zdbjq.cn/Article/details/guvgxkmcg.sHtML

[R12] for 遍历文件
来源：http://baike.zdbjq.cn/Article/details/guivhrynb.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.hesvh.cn/Article/details/gmvixfyed.sHtML

[R13] for 计数循环
来源：http://www.share.fehbvm.com/Article/details/geflnceeb.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.fehbvm.com/Article/details/ggoxcinzt.sHtML

[R14] C 风格 for
来源：http://www.m.share.hesvh.cn/Article/details/gnbdaexmi.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wap.hesvh.cn/Article/details/ghvahbgck.sHtML

[R15] while 逐行读文件
来源：http://www.share.zdbjq.cn/Article/details/gprtwwvyf.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.fehbvm.com/Article/details/gbliltvth.sHtML

[R16] until 等待条件
来源：http://wap.hesvh.cn/Article/details/gdyxtovyo.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.zdbjq.cn/Article/details/ggzfcadjh.sHtML

[R17] 数组定义与取值
来源：http://read.share.hesvh.cn/Article/details/ggnvbndch.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.hesvh.cn/Article/details/gafwwoagh.sHtML

[R18] 遍历数组
来源：http://wap.zdbjq.cn/Article/details/gwkanrcvn.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.fehbvm.com/Article/details/gafxafcve.sHtML

[R19] 数组长度
来源：http://baike.hesvh.cn/Article/details/glfxyccxk.sHtML

echo "${#arr[@]}"
来源：http://www.blog.fehbvm.com/Article/details/gfdizhhzp.sHtML

[R20] 关联数组（字典）
来源：http://3g.hesvh.cn/Article/details/gogmrrdda.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.fehbvm.com/Article/details/gixsoevod.sHtML

[R21] 字符串长度
来源：http://baike.hesvh.cn/Article/details/geashqsxj.sHtML

echo "${#s}"
来源：http://blog.zdbjq.cn/Article/details/gfsnwdfyi.sHtML

[R22] 截取子串
来源：http://www.share.zdbjq.cn/Article/details/gtwcjwjpi.sHtML

echo "${s:0:5}"
来源：http://read.share.fehbvm.com/Article/details/gardyqifh.sHtML

[R23] 字符串替换
来源：http://m.share.zdbjq.cn/Article/details/gfltjyqyw.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.zdbjq.cn/Article/details/gebqwmcym.sHtML

[R24] 大小写转换
来源：http://blog.zdbjq.cn/Article/details/gwdavrdyn.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.fehbvm.com/Article/details/gvunbwgyp.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.zdbjq.cn/Article/details/gfwnxxhqn.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.zdbjq.cn/Article/details/gxaycvhrx.sHtML

[R26] 命令替换
来源：http://3g.fehbvm.com/Article/details/gpjqwnrxt.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.zdbjq.cn/Article/details/gzwdcyego.sHtML

[R27] 算术展开
来源：http://m.share.fehbvm.com/Article/details/gkekmjkuq.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.hesvh.cn/Article/details/gsusbkeef.sHtML

[R28] 浮点运算
来源：http://baike.hesvh.cn/Article/details/gijcpqiln.sHtML

echo "scale=2; 10/3" | bc
来源：http://m.share.hesvh.cn/Article/details/gunokomve.sHtML

[R29] 定义函数
来源：http://read.share.hesvh.cn/Article/details/gzbdtkffk.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.fehbvm.com/Article/details/gpgjuzxfd.sHtML

[R30] 函数返回状态码
来源：http://baike.fehbvm.com/Article/details/gvlxsgndl.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.zdbjq.cn/Article/details/gyxxxgfhh.sHtML

[R31] 局部变量
来源：http://www.blog.zdbjq.cn/Article/details/grxcgnvjs.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.hesvh.cn/Article/details/gjkrkoehk.sHtML

[R32] 参数个数校验
来源：http://3g.hesvh.cn/Article/details/gbqpsayqw.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.hesvh.cn/Article/details/gpueblfhp.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.zdbjq.cn/Article/details/goczydilh.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.fehbvm.com/Article/details/gstjsqboy.sHtML

[R34] 退出时清理
来源：http://www.blog.fehbvm.com/Article/details/gzjzzroyz.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fehbvm.com/Article/details/gpbxxoqhd.sHtML

[R35] 后台执行并等待
来源：http://m.share.hesvh.cn/Article/details/gbppexsal.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.zdbjq.cn/Article/details/gorovfwtl.sHtML

[R36] 并发执行多个任务
来源：http://mobile.fehbvm.com/Article/details/ghbfapwqn.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.zdbjq.cn/Article/details/gmciqujuc.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.zdbjq.cn/Article/details/gpebnzpgl.sHtML

files=$(ls -1)
来源：http://wap.zdbjq.cn/Article/details/gsgabqrxw.sHtML

[R38] 管道串联
来源：http://www.blog.fehbvm.com/Article/details/gdmjbuyte.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.hesvh.cn/Article/details/grtejyfef.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.zdbjq.cn/Article/details/gxhpkfefm.sHtML

cmd > out.log 2>&1
来源：http://www.share.hesvh.cn/Article/details/gxjefjncx.sHtML

[R40] 追加写日志
来源：http://www.share.fehbvm.com/Article/details/gpoemvgdl.sHtML

echo "log" >> out.log
来源：http://3g.zdbjq.cn/Article/details/gikelaslx.sHtML

[R41] 丢弃输出
来源：http://m.share.fehbvm.com/Article/details/goememzah.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.zdbjq.cn/Article/details/glcpfvhyz.sHtML

[R42] 输入重定向
来源：http://www.blog.fehbvm.com/Article/details/gnnfoavba.sHtML

wc -l < a.txt
来源：http://baike.fehbvm.com/Article/details/gxykjpjap.sHtML

[R43] 按名字查找文件
来源：http://mobile.hesvh.cn/Article/details/gedykysia.sHtML

find . -name "*.log" -type f
来源：http://wap.hesvh.cn/Article/details/gkakglysl.sHtML

[R44] 按修改时间查找
来源：http://blog.fehbvm.com/Article/details/gqkbykhjc.sHtML

find . -mtime -7 -type f
来源：http://read.share.zdbjq.cn/Article/details/glgapabvg.sHtML

[R45] 批量删除
来源：http://wap.zdbjq.cn/Article/details/gqfrjvfcg.sHtML

find . -name "*.tmp" -delete
来源：http://wap.hesvh.cn/Article/details/gzwtplcuk.sHtML

[R46] 递归替换文件内容
来源：http://wap.hesvh.cn/Article/details/gkdiutwmu.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.zdbjq.cn/Article/details/gzavxduft.sHtML

[R47] sed 单行替换
来源：http://3g.fehbvm.com/Article/details/gbbnhimrc.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.hesvh.cn/Article/details/gdbcnxltm.sHtML

[R48] awk 取指定列
来源：http://m.share.zdbjq.cn/Article/details/gmszsnmmr.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.zdbjq.cn/Article/details/gpfnmbntg.sHtML

[R49] awk 带条件
来源：http://read.share.fehbvm.com/Article/details/glxbgauyw.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.zdbjq.cn/Article/details/gcyaskdqu.sHtML

[R50] awk 求和
来源：http://www.share.zdbjq.cn/Article/details/gwzpajldf.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.fehbvm.com/Article/details/geogpdfsc.sHtML

[R51] 排序去重取前几
来源：http://3g.hesvh.cn/Article/details/gnaztawmw.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.zdbjq.cn/Article/details/gsaiublnz.sHtML

[R52] 统计行数
来源：http://blog.zdbjq.cn/Article/details/gdcjwodat.sHtML

wc -l a.txt
来源：http://blog.fehbvm.com/Article/details/gledixcao.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.fehbvm.com/Article/details/gdnqrhnqi.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.zdbjq.cn/Article/details/gxrciebmi.sHtML

[R54] 比较两个文件
来源：http://read.share.fehbvm.com/Article/details/gmqphwnyn.sHtML

diff a.txt b.txt
来源：http://read.share.hesvh.cn/Article/details/geiscjgxc.sHtML

[R55] 压缩与解压
来源：http://www.blog.fehbvm.com/Article/details/glffdhugb.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.hesvh.cn/Article/details/gunfmjxbm.sHtML

[R56] 远程拷贝
来源：http://www.share.hesvh.cn/Article/details/gdjspfilf.sHtML

scp file user@host:/path/
来源：http://m.share.zdbjq.cn/Article/details/gjtozviez.sHtML

[R57] 远程执行命令
来源：http://mobile.hesvh.cn/Article/details/gfdbdbhln.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.zdbjq.cn/Article/details/gsclpqydw.sHtML

[R58] 下载文件
来源：http://mobile.zdbjq.cn/Article/details/gkbamlefl.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.hesvh.cn/Article/details/gbusbagvw.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.hesvh.cn/Article/details/ghmkhdzls.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.zdbjq.cn/Article/details/gbizzhzlx.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.fehbvm.com/Article/details/guyinrxjm.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.fehbvm.com/Article/details/glrxiuosh.sHtML

[R61] 磁盘占用
来源：http://baike.zdbjq.cn/Article/details/ghpcxoghb.sHtML

df -h;  du -sh *
来源：http://mobile.hesvh.cn/Article/details/gptbcxgum.sHtML

[R62] 找最占空间的文件
来源：http://read.share.zdbjq.cn/Article/details/gezsoowkw.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.fehbvm.com/Article/details/gakhjlbjd.sHtML

[R63] 内存与进程
来源：http://www.blog.fehbvm.com/Article/details/ghcqgdcxc.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.zdbjq.cn/Article/details/gtjljaikc.sHtML

[R64] 结束进程
来源：http://mobile.hesvh.cn/Article/details/gttllsirk.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.zdbjq.cn/Article/details/gnflzezba.sHtML

[R65] 查看端口占用
来源：http://m.share.zdbjq.cn/Article/details/gspidnvwj.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.zdbjq.cn/Article/details/gpybkwnqp.sHtML

[R66] 定时任务
来源：http://www.share.hesvh.cn/Article/details/gjnhdbsba.sHtML

crontab -e;  crontab -l
来源：http://baike.fehbvm.com/Article/details/gszmoelzx.sHtML

[R67] 生成随机十六进制串
来源：http://3g.fehbvm.com/Article/details/gjwnqowsv.sHtML

openssl rand -hex 16
来源：http://blog.zdbjq.cn/Article/details/ggmibkbls.sHtML

[R68] 计算文件校验值
来源：http://blog.zdbjq.cn/Article/details/ggkcoyjqf.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.hesvh.cn/Article/details/gldzqrons.sHtML

[R69] 生成随机密码
来源：http://www.blog.zdbjq.cn/Article/details/gutnspdvf.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.zdbjq.cn/Article/details/gvxdhpigr.sHtML

[R70] 时间戳与互转
来源：http://mobile.zdbjq.cn/Article/details/gqtymsdjb.sHtML

date +%s;  date -d @1700000000
来源：http://wap.hesvh.cn/Article/details/gneuesybw.sHtML

[R71] 日期格式化
来源：http://www.m.share.fehbvm.com/Article/details/gvifelodb.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.fehbvm.com/Article/details/gmgmfgnzd.sHtML

[R72] 等待端口就绪
来源：http://www.blog.fehbvm.com/Article/details/grohfdxtd.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.fehbvm.com/Article/details/gvjsjtadu.sHtML

[R73] 分割大日志
来源：http://mobile.fehbvm.com/Article/details/glphiubfb.sHtML

split -l 1000 big.log part_
来源：http://m.share.fehbvm.com/Article/details/gefstypwy.sHtML

[R74] 批量重命名
来源：http://www.m.share.zdbjq.cn/Article/details/gcawujool.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.fehbvm.com/Article/details/gsqdjapnx.sHtML

[R75] 导出环境变量
来源：http://www.m.share.zdbjq.cn/Article/details/gwjebunkb.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.fehbvm.com/Article/details/gxazqmxrn.sHtML

[R76] 使用临时文件
来源：http://mobile.hesvh.cn/Article/details/gufhnrprs.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.zdbjq.cn/Article/details/gkabnsshj.sHtML

[R77] 读取用户输入
来源：http://wap.hesvh.cn/Article/details/gyifbskly.sHtML

read -rp "请输入: " ans
来源：http://read.share.fehbvm.com/Article/details/gmeouqinx.sHtML

[R78] 交互式菜单
来源：http://www.m.share.fehbvm.com/Article/details/gcxxpibrw.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.zdbjq.cn/Article/details/ggvmeglaj.sHtML

[R79] 解析命令行选项
来源：http://read.share.fehbvm.com/Article/details/gjyzlambi.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.zdbjq.cn/Article/details/gpmsyhkfz.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.zdbjq.cn/Article/details/gyuhuxejj.sHtML

time ./run.sh
来源：http://read.share.zdbjq.cn/Article/details/gnaoszwxo.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gznmfsnon.sHtML

S. C / C++ 专题
来源：http://read.share.zdbjq.cn/Article/details/glbqvipci.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gisymvrfb.sHtML

[S01] C：Hello World
来源：http://www.share.fehbvm.com/Article/details/ghkjvegkn.sHtML

#include <stdio.h>
来源：http://www.m.share.fehbvm.com/Article/details/gvyrbznrr.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.zdbjq.cn/Article/details/gjjrsarwj.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.hesvh.cn/Article/details/ggpdpdkup.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.zdbjq.cn/Article/details/gfbdhkbkk.sHtML

[S03] C：读入整数
来源：http://read.share.zdbjq.cn/Article/details/gxgsuerkp.sHtML

int x; scanf("%d", &x);
来源：http://3g.hesvh.cn/Article/details/gvvxducaj.sHtML

[S04] C：字符串复制
来源：http://www.share.hesvh.cn/Article/details/ggnhdwkvf.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.hesvh.cn/Article/details/gkhlpiepl.sHtML

[S05] C：字符串长度
来源：http://www.m.share.fehbvm.com/Article/details/gyjhfxlpq.sHtML

strlen(s)
来源：http://baike.hesvh.cn/Article/details/gqpgycojh.sHtML

[S06] C：字符串比较
来源：http://3g.zdbjq.cn/Article/details/gbzvmzvxw.sHtML

strcmp(a, b) == 0
来源：http://m.share.hesvh.cn/Article/details/gjycwzkcg.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.hesvh.cn/Article/details/gmcwxjuak.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.fehbvm.com/Article/details/gnosxoyzq.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.hesvh.cn/Article/details/gdvvdizmy.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.zdbjq.cn/Article/details/geybathnw.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.hesvh.cn/Article/details/guimxeklv.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.fehbvm.com/Article/details/gqbfmbdcd.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.zdbjq.cn/Article/details/gtpnnfgwc.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.zdbjq.cn/Article/details/gfeomclmu.sHtML

[S11] C：逐行读文件
来源：http://wap.fehbvm.com/Article/details/gdshahked.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.zdbjq.cn/Article/details/gvjawfnhx.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.hesvh.cn/Article/details/gdqmitfwm.sHtML

fclose(f);
来源：http://www.share.zdbjq.cn/Article/details/ggspygmew.sHtML

[S12] C：写文件
来源：http://m.share.zdbjq.cn/Article/details/gounswlyk.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.zdbjq.cn/Article/details/gegocknnf.sHtML

[S13] C：宏定义
来源：http://read.share.fehbvm.com/Article/details/gmxlsoljs.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.fehbvm.com/Article/details/gelazwlja.sHtML

[S14] C：枚举
来源：http://mobile.fehbvm.com/Article/details/gkltdikmm.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.fehbvm.com/Article/details/ghpmsfgln.sHtML

[S15] C：类型转换
来源：http://wap.zdbjq.cn/Article/details/gbraiwddq.sHtML

(double) a / b
来源：http://www.blog.fehbvm.com/Article/details/gtvbrljvk.sHtML

[S16] C：位操作置位
来源：http://blog.zdbjq.cn/Article/details/gkgesvcmc.sHtML

x |= (1 << 3);
来源：http://baike.hesvh.cn/Article/details/gjslqkmtz.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.hesvh.cn/Article/details/grpufkzfk.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.zdbjq.cn/Article/details/gtxnsvkew.sHtML

[S18] C：命令行参数
来源：http://read.share.zdbjq.cn/Article/details/guidvnhzl.sHtML

int main(int argc, char **argv)
来源：http://m.share.hesvh.cn/Article/details/gvajwxpyc.sHtML

[S19] C：快速排序
来源：http://blog.hesvh.cn/Article/details/gdjeyexvm.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.zdbjq.cn/Article/details/guqlbstfg.sHtML

[S20] C：二分查找
来源：http://read.share.fehbvm.com/Article/details/gvlzkcvas.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.fehbvm.com/Article/details/ghizeolyc.sHtML

[S21] C：字符类别判断
来源：http://m.share.hesvh.cn/Article/details/gwtsoxwjj.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.hesvh.cn/Article/details/gxlamrvaz.sHtML

[S22] C：字符串转数字
来源：http://read.share.zdbjq.cn/Article/details/gxosfekpu.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.hesvh.cn/Article/details/gwdlwuacj.sHtML

[S23] C：随机数
来源：http://www.blog.hesvh.cn/Article/details/gpsytwskt.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.zdbjq.cn/Article/details/gvhegubji.sHtML

[S24] C：获取本地时间
来源：http://wap.fehbvm.com/Article/details/gqixmoxzr.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.zdbjq.cn/Article/details/gertamsxf.sHtML

[S25] C：内存拷贝
来源：http://wap.fehbvm.com/Article/details/gwgxjrxxr.sHtML

memcpy(dst, src, n);
来源：http://3g.hesvh.cn/Article/details/gccafuhtb.sHtML

[S26] C：内存清零
来源：http://www.m.share.hesvh.cn/Article/details/gdanleyea.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.fehbvm.com/Article/details/gebshcxft.sHtML

[S27] C：定义常量
来源：http://www.share.zdbjq.cn/Article/details/gcrznuhcu.sHtML

const double PI = 3.14159;
来源：http://blog.hesvh.cn/Article/details/goyfzijie.sHtML

[S28] C：静态变量
来源：http://www.share.fehbvm.com/Article/details/gcfgbuxsx.sHtML

static int counter = 0;
来源：http://blog.zdbjq.cn/Article/details/ghwesreeg.sHtML

[S29] C：变参函数
来源：http://wap.zdbjq.cn/Article/details/gzhzyxmcg.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.fehbvm.com/Article/details/gzxhldxug.sHtML

[S30] C：头文件保护
来源：http://www.blog.fehbvm.com/Article/details/grjaissux.sHtML

#ifndef X_H
来源：http://mobile.hesvh.cn/Article/details/grnppnxqw.sHtML

#define X_H
来源：http://wap.hesvh.cn/Article/details/gsfbvehdo.sHtML

#endif
来源：http://www.m.share.hesvh.cn/Article/details/gunlnuhrr.sHtML

[S31] C++：Hello World
来源：http://baike.hesvh.cn/Article/details/gzsbaihoo.sHtML

#include <iostream>
来源：http://wap.fehbvm.com/Article/details/gzbnicnoa.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.hesvh.cn/Article/details/gndsojmae.sHtML

[S32] C++：字符串
来源：http://wap.fehbvm.com/Article/details/gyypabxgo.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.zdbjq.cn/Article/details/gwjesegcu.sHtML

[S33] C++：vector 增删
来源：http://m.share.zdbjq.cn/Article/details/gbuosxbpu.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.fehbvm.com/Article/details/gismfqobh.sHtML

[S34] C++：遍历 vector
来源：http://m.share.zdbjq.cn/Article/details/gchuahrqi.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.fehbvm.com/Article/details/ganljmwxy.sHtML

[S35] C++：map
来源：http://m.share.hesvh.cn/Article/details/gchngictp.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fehbvm.com/Article/details/gjvngidpx.sHtML

[S36] C++：unordered_map
来源：http://3g.zdbjq.cn/Article/details/gsbizktco.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.zdbjq.cn/Article/details/gvcqiyppl.sHtML

[S37] C++：set
来源：http://m.share.zdbjq.cn/Article/details/ggtsifxmh.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.hesvh.cn/Article/details/glkdikrds.sHtML

[S38] C++：排序
来源：http://mobile.hesvh.cn/Article/details/gzmhajzsw.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.hesvh.cn/Article/details/gfzppqlet.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.fehbvm.com/Article/details/gasrrsapa.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.fehbvm.com/Article/details/gocyybwfo.sHtML

[S40] C++：查找元素
来源：http://3g.fehbvm.com/Article/details/gccmidkqu.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.zdbjq.cn/Article/details/gqvrbqosk.sHtML

[S41] C++：类与构造函数
来源：http://blog.hesvh.cn/Article/details/gmiwwsjez.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.fehbvm.com/Article/details/gssihkryk.sHtML

[S42] C++：继承与虚函数
来源：http://3g.hesvh.cn/Article/details/gpenulndu.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.fehbvm.com/Article/details/geoqfzgsd.sHtML

[S43] C++：智能指针
来源：http://www.blog.hesvh.cn/Article/details/gbwpuihcb.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.hesvh.cn/Article/details/gyskylmcv.sHtML

[S44] C++：引用传参
来源：http://blog.fehbvm.com/Article/details/gnjuselgy.sHtML

void inc(int &x) { ++x; }
来源：http://3g.fehbvm.com/Article/details/grvwncstq.sHtML

[S45] C++：lambda
来源：http://3g.fehbvm.com/Article/details/gzdlayegu.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.hesvh.cn/Article/details/gaodmxcpc.sHtML

[S46] C++：函数模板
来源：http://m.share.fehbvm.com/Article/details/gkrdilgce.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.fehbvm.com/Article/details/gnsluofhg.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.zdbjq.cn/Article/details/gutoywpha.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.hesvh.cn/Article/details/gvbrdzwos.sHtML

[S48] C++：逐行读文件
来源：http://baike.hesvh.cn/Article/details/gxhbdrrpv.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.zdbjq.cn/Article/details/gbrzmnriz.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.hesvh.cn/Article/details/grwnmtxdl.sHtML

[S49] C++：写文件
来源：http://3g.fehbvm.com/Article/details/gzbfelhoe.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.zdbjq.cn/Article/details/gbfshsdoz.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.hesvh.cn/Article/details/gktsjausz.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.zdbjq.cn/Article/details/gkhjfcdlc.sHtML

[S51] C++：显式类型转换
来源：http://m.share.fehbvm.com/Article/details/gfklznxfe.sHtML

static_cast<double>(a) / b
来源：http://www.share.hesvh.cn/Article/details/goifhchif.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.hesvh.cn/Article/details/gakyhadmc.sHtML

int size() const noexcept { return n_; }
来源：http://blog.fehbvm.com/Article/details/gfgbpikfg.sHtML

[S53] C++：移动语义
来源：http://wap.fehbvm.com/Article/details/gemwbgukg.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.hesvh.cn/Article/details/ghypgsfvz.sHtML

[S54] C++：异常处理
来源：http://www.m.share.zdbjq.cn/Article/details/gzblgomvc.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.hesvh.cn/Article/details/gmfmlreyv.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.zdbjq.cn/Article/details/gjwemsvpj.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.zdbjq.cn/Article/details/gvmvevgqs.sHtML

[S56] C++：optional
来源：http://mobile.zdbjq.cn/Article/details/gfcoygoge.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.zdbjq.cn/Article/details/geizxynga.sHtML

[S57] C++：编译期常量
来源：http://www.blog.hesvh.cn/Article/details/gkvjashbu.sHtML

constexpr int N = 10;
来源：http://3g.zdbjq.cn/Article/details/gkaucupwg.sHtML

[S58] C++：命名空间
来源：http://blog.hesvh.cn/Article/details/gujtrhqxh.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.fehbvm.com/Article/details/gtxszcdgs.sHtML

[S59] C++：静态断言
来源：http://wap.zdbjq.cn/Article/details/gyzsetmtj.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.zdbjq.cn/Article/details/ghgubnfqk.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.hesvh.cn/Article/details/gmpipmihh.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.zdbjq.cn/Article/details/gqfelhiyj.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gggdhuqzy.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.fehbvm.com/Article/details/gotrphhyk.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/ggymobkpa.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.fehbvm.com/Article/details/gqtfkdupz.sHtML

println("Hello")
来源：http://read.share.hesvh.cn/Article/details/gqqzbuhdo.sHtML

[T02] Kotlin：变量
来源：http://mobile.fehbvm.com/Article/details/gvntendrv.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.hesvh.cn/Article/details/gekfukxpr.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.hesvh.cn/Article/details/gzpafcssr.sHtML

"值: $b"
来源：http://mobile.hesvh.cn/Article/details/gcoojqdws.sHtML

[T04] Kotlin：空安全
来源：http://read.share.fehbvm.com/Article/details/glrjmzdem.sHtML

val n: String? = null;  n?.length
来源：http://www.blog.fehbvm.com/Article/details/gpsvmuloi.sHtML

[T05] Kotlin：when 表达式
来源：http://mobile.hesvh.cn/Article/details/gttkohdaz.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.fehbvm.com/Article/details/ghbvnyvpw.sHtML

[T06] Kotlin：集合映射
来源：http://blog.zdbjq.cn/Article/details/gqfqmvlsl.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://blog.zdbjq.cn/Article/details/gieavfrsb.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.fehbvm.com/Article/details/gcgoafvhp.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.hesvh.cn/Article/details/gubeujenj.sHtML

[T08] Kotlin：数据类
来源：http://m.share.fehbvm.com/Article/details/gvzujuicg.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.fehbvm.com/Article/details/gjdtcxmnf.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.fehbvm.com/Article/details/gdqqsaxrk.sHtML

fun String.exclaim() = this + "!"
来源：http://blog.fehbvm.com/Article/details/guaycpiss.sHtML

[T10] Kotlin：默认参数
来源：http://3g.zdbjq.cn/Article/details/gdlcofdhm.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.hesvh.cn/Article/details/gcppgwpyb.sHtML

[T11] Kotlin：协程
来源：http://blog.hesvh.cn/Article/details/gkzljobec.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.fehbvm.com/Article/details/glpvrtuzm.sHtML

[T12] Kotlin：解构声明
来源：http://baike.fehbvm.com/Article/details/gdlozzweb.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.fehbvm.com/Article/details/gkfoatpir.sHtML


<!-- 参考信息 -->