代发 wailian999

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3anbikhqb.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3cdovmlqp.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3zjiaiyac.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3hmdagklu.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3kpflexgg.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3jpswtuzb.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3ytoqalmn.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3nrquwxjl.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3cgkdzpcb.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3fljayrdr.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3tpoxarcp.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3vbqgtllk.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3onafxers.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3cotojqse.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3scbtcrwu.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3azxyhadf.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3cfvtcyul.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3dgqivdgd.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3xskwrahz.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3bawsdnie.html

esac
来源：http://www.52xcode.cn/Article/details/gt3pxdyvubu.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3zndntfsb.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3ftufrjeo.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3ninxyxwn.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3dckvpxxc.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3pnleueag.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3ytqtrnpn.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3ycjszbho.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3azqqsfva.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3mgogrlpe.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3gdhkfbuk.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3zbfxnkhz.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3nmkpjtua.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3ufukvcqu.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3diemfrya.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3zlqfquxi.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3zvyeqmww.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3opxmdktr.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3hyxwtcsi.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3wajqfxaf.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3wtbifstw.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3rtlnmdnt.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3rmcaebtv.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3xsqwxsph.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3ozkkmbkq.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3pqakduuf.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3gmssyqwd.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3mkzagohg.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3jdhwflws.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3kaovyrta.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3wupgpczu.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3qmbvdftz.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3xtliuile.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3kzqpnmzh.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3sqackvfm.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3hwrgiidi.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3blezbddl.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3aiildtuf.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3suarjyfg.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3nrnrsyjl.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3uswygztx.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3qwnqxfrq.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3ihvwhtkk.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3thnrxqrl.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3jnwvdsju.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3cwvgwjbj.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3bsaowxhz.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3hjzgvsbf.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3nhnowekv.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3qyndmopo.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3ajukbdso.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3demmxxcs.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3kedffeom.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3gnlyzlhk.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3fljlvuca.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3rbcvedrg.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3wlzskxka.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3agroiknq.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3prcgwusg.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3ymdemfhp.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3prgbvfea.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3ycjxuefj.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3iaieidan.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3fdcjzeye.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3uqdmlpvd.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3xecxbbmu.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3gmoujwqr.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3wikxiajl.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3vvuxpxil.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3pjcmwsqn.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3qbqrtxbk.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3paxphzsi.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3oeogrfit.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3yklgdxpm.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3tiiyzahi.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3xyisgnro.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3dwoyrpjf.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3pywanwjf.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3uakhdjvr.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3cligzohx.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3jqcdyivk.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3oxzeuebb.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3wuxectfb.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3ypzwxmqi.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3mskcfdyz.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3egpeqjga.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3lwmthoov.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3zhpvpydr.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3logzxyle.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3guqfgznk.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3mwppgsaq.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3dupeqygq.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3hsjeywmu.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3xpweyfoz.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3dkijvqyc.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3gibxpdbv.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3ojnggvje.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3uwcsddft.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3gxwsgzjj.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3xaklcdwl.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3owtvxxqi.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3csbczfhb.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3zfgspovq.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3vygynnvq.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3eygyissr.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3bfjtbvcz.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3gbhfudpc.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3fubetyyw.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3imzxjvwe.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3gsnhsvif.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3wpquhyhk.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3pniqqeeh.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3yggviyfb.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3ewbalsyi.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3uhozbjjq.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3qcwivfll.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3xflwmbra.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3xepiuuih.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3prfwwmxd.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3crtrelhh.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3xsdcbbax.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3fcjaautm.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3capbdhep.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3zayndzqt.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3ehzalvuz.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3perxgnpl.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3zgzmrjll.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3zcsqwzfa.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3wuywghmc.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3utchducl.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3qhbezjgo.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3epreyqar.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3qsenuzdq.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3whirlilu.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3knhyemco.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3vvnsktej.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3kexddfxs.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3ltpfglxk.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3amvdxuzk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vxahjirs.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3zwawquje.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tqqixflq.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3mivizqao.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3zbsiopkn.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3nnottbql.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3jqrigohx.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3rmqgnrmx.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3twaylftz.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3qpedbswu.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3tmqqwssq.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3abtktzdf.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3ukcesnkp.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3eyxyzmez.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3rzbyhmpe.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3xeafaskg.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3luqdzger.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3zsvaknuv.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3xcubczay.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3ojjibkjr.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3yfpmtrfm.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3pieebazg.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3myvrxxjs.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3fdpuaexm.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3tkiscduq.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3ksdwutfq.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3osnssnio.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3mcmmbsig.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3atkdakvi.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3fvhgkntv.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3fvkxaekq.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3qkidsofo.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3tgffqozk.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3dykknnxv.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3yizopmyc.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3oqhgblli.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3kuyesxfk.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3uhywtqde.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3xmotqquv.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3hjfrrcfq.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3oseslihl.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3nujbcyyb.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3wqhzysuu.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3oflgrmah.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3nxrpsycn.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3hxkxjrxh.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3lwrrifti.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3vadntmkn.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3rzxtxqml.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3rgytbqpo.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3qtotrakj.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3zfzmnhme.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3cfbmqudk.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3hetnfuke.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3evjruuyl.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3wtmaazaw.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3foflmdri.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3mhwulaua.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3izgmrlvs.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3gqhfwiwo.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3ehbyyweu.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3owhnjsrd.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3kulexveb.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3bsfjesqf.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3mxuhasbf.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3rjvposdf.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3yvxnrkrc.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3ukjiqpsk.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3mmbdntms.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3dtjnnxir.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3gbwurhmp.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3uitfnftr.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3gfqsmtpt.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3cjqhijhr.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3fslkpqck.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3fltxxcds.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3rftnooxn.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3qyhdkdsz.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3qlxlwjxv.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3iiagfzoz.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3tspfyafz.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3exdzhceb.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3dvnmxwry.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3nuhuhhcf.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3arfwbxle.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3svzblaxl.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3ojvkjuzl.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3klyxmgsv.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3xsfbwgxz.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3neuxzaid.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3dktrronj.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3rymbbtec.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3jcokfkol.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3qnzbxtos.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3lzxbgywf.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3zqtullhm.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3bntgrgys.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3fwpfehqe.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3lsdnqoea.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3pojvvvvz.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3sdtkhnul.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3senxrqxu.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3gkpmixxe.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3gfhemvat.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3gpkfkqtc.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3hqcwjcyt.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3cmofmeuc.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3deenfsjb.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3bmmpazsq.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3tthbcapj.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3dnqgnwfl.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3sohikgcj.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3xmvmsraw.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3ngbtpirw.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3thgiiwer.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3sofxvtnk.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3xpgrxrah.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3efvvwjtb.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3macofbxw.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3sjyihydb.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3faqrvgys.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3hcmhlwwe.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3zigvauqm.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3ykulrgdv.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3wuqkzpfd.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3esfjhmiw.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3hoisrjlc.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3cufddgoz.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3dqsrmdkr.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3ysvjpzbm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xmvcjekg.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3nztmqlfv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3omzigpxl.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3zisxazih.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3avjpvhyj.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3gwzwuujt.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3pgvdclfd.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3jcifvucy.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3vhhogvws.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3xaqavsat.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3cmjqgtor.html


<!-- 参考信息 -->