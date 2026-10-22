代发 wailian999

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2mdoiydcc.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2xjfmcepi.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2lmtteagb.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2qbzzvneo.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2gtvzftui.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2zitiwgac.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2wckbitse.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2pvbidvwp.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2zgxiddww.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2ynscefbj.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2dyirdmbz.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2prtbwirs.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2qinowddz.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2lqmfjjmd.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2qkrkfbnf.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2ryacahyn.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2swnchfct.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2tirfbduz.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2fvqrawbd.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2oycdrqdt.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2jycjrrwt.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2brxzbsco.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2pfwyyxlj.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2pvhtqyqr.html

esac
来源：http://www.52xcode.cn/Article/details/gt2mutvahyd.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2cxyoobce.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2wzkurndy.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2cfzkelut.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2wbqyzvfx.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2gmabvavg.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2lgohevjf.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2fjjlmsrt.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2qyhwurni.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2rhsmjcin.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2jxowckwx.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2vwrsxtyp.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2wdirupbv.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2jcrzmnwl.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2oiextpsr.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2tbbebipk.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2eucwvqtq.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2immwxdox.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2pqtvbzjq.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2ehihlyta.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2elaoodwn.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2rxhudspi.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2khsbruvv.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2bmihouxh.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2jfoxvynp.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2rwcmwrdd.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2izkvbwgt.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2sydhbpbe.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2zalrzahi.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2bfozeazq.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2dcxgjren.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2vxphcyph.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2skfvywaz.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2bgialeji.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2zvinztfv.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2xsnemclk.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2djqjpfyw.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2ocayskqr.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2amfxkbcn.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2ujkxbpjo.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2xlxlmmul.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2dnfaoamx.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2yonriski.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2hvqwnvmd.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2fcwsjxlj.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2ytyvbgcr.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2xwpxrpju.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2kuouridy.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2hwprkkgg.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2ehgplwjd.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2wbtidqju.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2lttfgqwg.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2gbxjvbmq.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2oittgexd.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2pprhzcdu.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2wxlrzcxu.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2obiygwtb.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2ltdxumbf.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2kqumethl.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2tpiwrrby.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2omcigsba.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2stsqyapi.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2nsukzibv.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2nueiztau.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2twjkyhjj.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2lpxmvrjw.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2ovltcunj.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2omonsivt.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2gegelklc.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2iwdygppy.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2jquqjerh.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2gzjqekgi.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2zrtvtcjk.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2upeyuwnc.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2jjwthlph.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2mhmgbyur.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2rlbnemkx.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2sddifqes.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2wymalnac.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2alsdnfra.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2naolznum.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2zirjhpjx.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2qkkiauch.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2niupvqqz.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2jhchuycn.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2tehafjud.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2tjxhwjaj.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2lqwlrjpf.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2foxdtirv.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2kgvzpyjq.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2nxkskchp.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2uqzszboz.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2lqolrpbo.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2ielsosmq.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2nddvokoi.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2nmmwiedc.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2yyxeffrp.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2syslefxs.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2uphhigzv.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2svqorzsk.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2frzdkqer.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2etmbhglt.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2axpujttj.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2gspilkps.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2wewquvka.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2nnyjoqnt.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2titzkqkh.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2fhiaragw.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2evitpzej.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2lxyqirjh.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2tqptrwtq.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2mdpmwtou.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2iepgklhd.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2wdlbzvox.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2blafzfve.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2cztjyttn.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2imtecjee.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2tmclfmxt.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2bjokpfnh.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2tbohyesq.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2ppnedqfj.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2lpnsljia.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2hxwtrocr.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2ikkgfvyc.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2wxfzfyhx.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2pfduqrlg.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2quabpcpn.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2kmeguxdi.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2nywfnnoe.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2gxuuhpyf.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2aibhszfn.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2dgfnkjss.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2xdfhfmsg.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2qlgmbbqu.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2rkzjezfj.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2yenxzvrd.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2ybfxgbnr.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2eojyimap.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2hhlgucfs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yydhnojv.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2wvzckxko.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2sngpvfmk.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2bxqnrkym.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2qwatxyac.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2wvlftozr.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2hmxfdbcf.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2cljsuuek.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2afxhvyos.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2vriqvpnt.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2rkwiikeu.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2urlwbejp.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2mdsfriox.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2rmeohmvf.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2rhowneij.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2hkdcviok.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2gumpccgy.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2yvsiwmqm.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2lmkqfuiy.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2wluzgzbw.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2zrpmukjr.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2lybknhjd.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2lkmwpjfv.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2gyddkmgj.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2actnlnkm.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2pjtkbwlw.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2waeoyzkf.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2pxxafrgp.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2kilirkyw.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2pitlnbdv.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2catlqtal.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2fmfluxot.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2oruolhlh.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2yowdvblk.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2bmelcdrw.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2iokgxfau.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2ceqqgtaa.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2njghiiyx.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2wjxlqimf.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2rbpyudvj.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2izmsflpd.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2iilavahq.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2mjxoaqcu.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2sutojlsg.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2hwnsdcrf.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2pgykfmzf.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2jzqmaqbe.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2dggrlvyr.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2mtetroko.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2ssawmzmb.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2cnnrxyyb.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2iwzrmlrd.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2qtvbvcze.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2bqgqyyxn.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2zgrzjqwr.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2zortflbg.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2jssexsix.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2jwaztapi.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2dmeunopd.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2jxvytvne.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2htfftwal.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2blilnkia.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2ptkvlfkk.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2ojlsmydb.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2uwswzgkq.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2nyrksrjl.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2mcxykpik.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2sfozqsbm.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ejtfwbkn.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2mtyxjjhm.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2bzenewxk.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2tvdtcxgd.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2xjxtivzt.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2aywwjavh.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2dsxotusx.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2zuygsyyb.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2tvwpwvap.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2dhwjpruz.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2jxpdwbxp.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2dvonoggw.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2ptzgwdob.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2qscnfkvb.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2hrsndxpr.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2gzohwpyj.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2ujpqwtes.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2cjxjvaqu.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2ctsbnfys.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2mdptgbpj.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2vrudxzvh.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2jvbjpeqd.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2kujnxqbk.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2vwbpbibh.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2alnneajs.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2apejlqnu.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2orosbuuw.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2dpuabixc.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2iwbdcorb.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2ddknsgpq.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2flswjnjw.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2xvjzdrpm.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2mpohopui.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2kxpgrzol.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2tjyypljy.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2zhghzivw.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2jubexziy.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2oxmhypdo.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2lvuratxm.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2pjiclfan.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2utvgcrxd.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2qztldvgz.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2bgqcfomn.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2ppmhgtuz.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2yajdklat.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2amhkwipi.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2moghkwur.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2oystpbyq.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2pnicfaeb.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2qbbjdnwv.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2lbophavn.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2meoovxkn.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2uvtnduie.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2wojjhstg.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2wfhwqrfv.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2vvhkodfw.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2qjphgyzm.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2lxiccgqj.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2mopfznzj.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2atulethq.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2lbqjbrku.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2aoegfial.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2acybxobf.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2tqvihefu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2aiupfhfd.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2xzfyfxwc.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2mjbarfud.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2dwdzhchx.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2vhwqbsgk.html


<!-- 参考信息 -->