代发 wailian999

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2dvzlcyim.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2ocudllsj.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2iugsflry.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2wsigittg.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2jqghkllo.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2hckobpet.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2ihcygotf.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2osuknacq.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2djtqfjnq.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2vppeaosa.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2mimyxouk.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2zmlouxal.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2uizqctww.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2whfektuk.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2stamsvjh.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2gcingagc.html

esac
来源：http://www.52xcode.cn/Article/details/gt2fdoyjltg.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2jlsytudj.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2muilmoim.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2zjkcidlr.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2jyqtzchs.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2raekyhrb.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2henrmnxs.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2kjmsoswg.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ixoazfmo.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2klctxhxb.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2nzmzrduw.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2grgshhfv.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2alvoiqlo.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2heofikhg.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2yaemjbrq.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2owgiexcl.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2tnjevdpb.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2esozioon.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2xfjyykms.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2wxzducxo.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2jmfgnohj.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2hcqwqjyu.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2mcdimpia.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2dssplmxc.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2itnhiubg.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2aemaixji.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2xzjfdefi.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2iueteclf.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2vqinyqjq.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2szwswlyc.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2wwubrcwo.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2bmkyzhjy.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2rtknrydj.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2jbnnbkrb.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2miaaeumb.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2ismgbfym.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2bolzxxlx.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2evadwbqy.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2ykyiqqih.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2zfudzsdr.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2wwpugrtx.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2ohveryti.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2dewvejbk.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2qgmpxddd.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2nfnuwfbb.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2jvxkkfew.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2ajiyoahm.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2nwoqlkmf.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2aevxggqw.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2fsorqdwm.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2nofwjawq.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2xhdliavi.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2ejqzcwdl.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2juolboqc.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2vgiccsga.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2izaaphpq.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2wehnsfey.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2spvbjrzu.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2mlgqispn.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2shleblzd.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2wxeeyakc.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2oiqstkjy.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2vuitgjgc.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2szbftmsc.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2ilhpxjoc.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2ypkomqza.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2sjliacat.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2jzrfwodg.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2dnckwkuz.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2cxvczrpv.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2fxkhhyhm.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2lmapkqkz.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2adpdryoy.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2utimyxsw.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2wogstlbw.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2tmmtpjpi.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2pdhveate.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2bmqtusaz.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2gavbnork.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2rdeuvphp.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2toxkcecg.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2tminqqiq.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2wbijtoej.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2nyisnobp.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2tltzfjvg.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2zzzgbrgm.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ripofdyb.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2agloguqu.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2dduegbhm.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2vlogtzem.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2hmvambfk.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2srjkamxw.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2nbwythcj.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2hydbqwce.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2ikuguxkj.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2xlpbxfkd.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2ocphghpg.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2behylphk.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2oojyyuqr.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2wjbdzvqe.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2immvblma.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2ldnbsmur.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2wyuxdpct.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2isthavds.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2kmcokgwk.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2gjwcldvr.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2ndosvjxz.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2qbuajigp.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2uhumkrpw.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2bnudpxka.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2jjhzfmkv.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2pylhlljq.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2txaalnmn.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2rrmopgqf.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2olhhvxwz.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2xwbnjmxb.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2torimhub.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2kkujeeca.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2xbfotenp.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2ckmizigw.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2ovgdlxbf.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2gsbyqyvf.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2mwbduqww.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2nfkwucos.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2iswxfvsy.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2rypbyqhu.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2emhrlcxt.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2vjpixmdz.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2eheaujxu.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2gckiewhm.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2xhwwncah.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2rnovqbqa.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2wbludren.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2iixonlwk.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2yzydmlrp.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2swnuhuif.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2xqmgayto.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2pwvblhfd.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2geuhryig.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vzeffnhh.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2tmmrbdpl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dxubmomr.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ykmygijx.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2qhbtmbof.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2hnlkatps.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2ywmxckqz.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2slzrrtbr.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2hxvzvkyz.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2nvwlkdad.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2qboxhvnm.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2lvvlzxof.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2suezqpsx.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2dcugebgj.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2rpirxdsj.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2duelistb.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2okdqntiw.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2oeiygyax.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2wrjdkgjt.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2ubfpzwnd.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2eqlovofl.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2tzdosuql.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2gvwihwrx.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2pyjviyue.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2aualxwrh.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2zfkuvaea.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2bavhtznq.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2kpmjvefh.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2ucptpoar.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2hurqcvxa.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2afzphxto.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2uhzwzyks.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2akoflunt.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2nprlkrhj.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2ygnwentk.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2jrjjjawh.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2yfkpoisq.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2jrdjgpyk.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2atggnikx.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2cxnwuxvr.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2iusugzfb.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2ooxkexsl.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2ucbftogb.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2rhdshapa.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2ggqphjcn.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2bzpavqbn.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2poowsyce.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2ubqfttyf.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2uthwbnny.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2slpjpavs.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2rfxyfuxt.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2wyzxnlst.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2jdqdzmbb.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2kndufmqk.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2mkmrrdkq.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2rhidrcut.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2fqjbnuwv.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2clkvpmap.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2rgompwij.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2hfvmcayh.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2wtlmjdrz.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2nfiirwon.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2gfknqxyb.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2ezynuxmh.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2dxwqarnl.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2zsocdepu.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2fwdrfbkw.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2ojtfwckw.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ajdlkywq.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2tcmjjgig.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2jcmtznmv.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2samynjpa.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2wjstkwfj.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2aaxcfpxj.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2lhcrjlwa.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2asxbgwhb.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2ovuvrgzl.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2uvpyczse.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2dochadnc.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2pqipfwfy.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2ngmykxtu.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2oetnrwxn.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2rxlodhsa.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2bxwwsluv.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2lceflyxk.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2huqnvkes.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2smhdjtil.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2mlxlqhta.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2zkdvlcjh.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2rtcyjbim.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2vsrkifuw.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2vqxeigxa.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2nrqjvhua.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2phywrftf.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2ovijwqck.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2nuwvuubl.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2nkvannbh.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2gxdrsvlu.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2gaciubyx.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2zfbqragw.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2viepzght.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2xnnukaka.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2cxvkdjzz.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2ccskqujq.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2htlupbdl.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2fjquaobi.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2akwtcjha.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2yzgqnluf.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2jybvufxw.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2zizixjbg.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2atayhhcg.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2zbvxvikh.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2iaigdryn.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2gqsmganw.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2nestkbzk.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2hdkyujbl.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2uqcyxknp.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2foxlozok.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2qjhnimyk.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2hjbaozti.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2puoebuwm.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2wspfxfin.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2pnyfcwic.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2hkupnvhn.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2rfwueeji.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2hzbukneb.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2bckbdyss.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2kxmnepro.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2bplnhphm.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2jmeprvih.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nxbwpfxy.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2vrbymkqz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fgljdtrs.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2uxdgvcal.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2tqrzyuua.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2shsccrgg.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2oseujgmy.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2frzmdqir.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2pxixvvss.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2iiokbghz.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2zsshlozi.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2qggruwcg.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2gwnvqsjs.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2tccdgqzt.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2owazzfzk.html


<!-- 参考信息 -->