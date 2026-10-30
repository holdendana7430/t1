代发 wailian999

set -euo pipefail
来源：http://m.share.zdbjq.cn/Article/details/ghnuivcaf.sHtML

[R02] 变量赋值与使用
来源：http://m.share.fehbvm.com/Article/details/glgrvtefv.sHtML

name="Tom"; echo "$name"
来源：http://blog.fehbvm.com/Article/details/gnizxxwrm.sHtML

[R03] 只读变量
来源：http://www.share.zdbjq.cn/Article/details/gxjdeqcmb.sHtML

readonly PI=3.14
来源：http://baike.hesvh.cn/Article/details/gemjbbgdo.sHtML

[R04] 位置参数
来源：http://baike.zdbjq.cn/Article/details/gjicfhmkg.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.fehbvm.com/Article/details/gealvlxbz.sHtML

[R05] 参数默认值
来源：http://read.share.hesvh.cn/Article/details/ghfeglorq.sHtML

name="${1:-default}"
来源：http://m.share.fehbvm.com/Article/details/gwqhljrhb.sHtML

[R06] 判断命令是否存在
来源：http://3g.zdbjq.cn/Article/details/gogoyzevw.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.zdbjq.cn/Article/details/gwyeaqaft.sHtML

[R07] if 判断文件
来源：http://blog.fehbvm.com/Article/details/gkkcmaodt.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.fehbvm.com/Article/details/gxxjoxhgs.sHtML

[R08] 数值比较
来源：http://wap.hesvh.cn/Article/details/gaessvdum.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.fehbvm.com/Article/details/gwgzuhark.sHtML

[R09] 字符串比较
来源：http://www.blog.fehbvm.com/Article/details/gghlyttfz.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.zdbjq.cn/Article/details/gjfqxendc.sHtML

[R10] 正则匹配
来源：http://baike.hesvh.cn/Article/details/gkmpunhjn.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wap.fehbvm.com/Article/details/giohznkbc.sHtML

[R11] case 多分支
来源：http://www.blog.fehbvm.com/Article/details/gnqykbkto.sHtML

case "$1" in
来源：http://3g.hesvh.cn/Article/details/gpukwaenw.sHtML

start) echo "启动" ;;
来源：http://m.share.fehbvm.com/Article/details/gsheuvsmz.sHtML

stop)  echo "停止" ;;
来源：http://3g.fehbvm.com/Article/details/gnogceidi.sHtML

*)     echo "未知命令" ;;
来源：http://www.share.hesvh.cn/Article/details/gwqzfymvx.sHtML

esac
来源：http://blog.zdbjq.cn/Article/details/gowfonbgl.sHtML

[R12] for 遍历文件
来源：http://m.share.zdbjq.cn/Article/details/gskzhwxqg.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.fehbvm.com/Article/details/gzutyoxla.sHtML

[R13] for 计数循环
来源：http://3g.zdbjq.cn/Article/details/ghgqkjxun.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.hesvh.cn/Article/details/gyntmqaou.sHtML

[R14] C 风格 for
来源：http://www.blog.zdbjq.cn/Article/details/gfvoznkcm.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://baike.fehbvm.com/Article/details/gdwlwyiks.sHtML

[R15] while 逐行读文件
来源：http://www.blog.fehbvm.com/Article/details/ggbagwjmx.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.fehbvm.com/Article/details/goqjqmhaw.sHtML

[R16] until 等待条件
来源：http://read.share.fehbvm.com/Article/details/gritxsilz.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.hesvh.cn/Article/details/gqgdsqvnt.sHtML

[R17] 数组定义与取值
来源：http://read.share.zdbjq.cn/Article/details/ghvhjygfq.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.hesvh.cn/Article/details/gxtymvioo.sHtML

[R18] 遍历数组
来源：http://baike.fehbvm.com/Article/details/ghaxnvqmk.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.m.share.zdbjq.cn/Article/details/ghtcxinvb.sHtML

[R19] 数组长度
来源：http://mobile.hesvh.cn/Article/details/gcpnijqcv.sHtML

echo "${#arr[@]}"
来源：http://read.share.zdbjq.cn/Article/details/gtgicrtvz.sHtML

[R20] 关联数组（字典）
来源：http://baike.hesvh.cn/Article/details/glerznpqj.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.zdbjq.cn/Article/details/gfnimkbxk.sHtML

[R21] 字符串长度
来源：http://mobile.fehbvm.com/Article/details/gcrupkygp.sHtML

echo "${#s}"
来源：http://m.share.zdbjq.cn/Article/details/gaqqazmzt.sHtML

[R22] 截取子串
来源：http://baike.hesvh.cn/Article/details/gntgmsqoh.sHtML

echo "${s:0:5}"
来源：http://m.share.fehbvm.com/Article/details/glsmjdcnh.sHtML

[R23] 字符串替换
来源：http://www.blog.zdbjq.cn/Article/details/gripgsjwi.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.hesvh.cn/Article/details/gpkldmznh.sHtML

[R24] 大小写转换
来源：http://www.blog.fehbvm.com/Article/details/ghlueuqkv.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.hesvh.cn/Article/details/gsspvgvbk.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.zdbjq.cn/Article/details/givbqohaz.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.hesvh.cn/Article/details/glzglcncf.sHtML

[R26] 命令替换
来源：http://www.m.share.zdbjq.cn/Article/details/giiwxswyb.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.hesvh.cn/Article/details/gqkgbtirt.sHtML

[R27] 算术展开
来源：http://m.share.zdbjq.cn/Article/details/gvxttzsjy.sHtML

echo $((1 + 2 * 3))
来源：http://wap.zdbjq.cn/Article/details/gyytcmdnz.sHtML

[R28] 浮点运算
来源：http://wap.fehbvm.com/Article/details/ggwhahgjs.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.zdbjq.cn/Article/details/gwyfhyofq.sHtML

[R29] 定义函数
来源：http://www.share.zdbjq.cn/Article/details/gxtravwnh.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.zdbjq.cn/Article/details/gbigfpkvs.sHtML

[R30] 函数返回状态码
来源：http://www.share.zdbjq.cn/Article/details/gbnqlikyx.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.zdbjq.cn/Article/details/gjupfwbqa.sHtML

[R31] 局部变量
来源：http://wap.hesvh.cn/Article/details/gutseybur.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.zdbjq.cn/Article/details/gcnxxtliu.sHtML

[R32] 参数个数校验
来源：http://read.share.fehbvm.com/Article/details/gbpdanvbd.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.zdbjq.cn/Article/details/gkxpzdglx.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.hesvh.cn/Article/details/gyekoprxm.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.hesvh.cn/Article/details/ghvmjbhrn.sHtML

[R34] 退出时清理
来源：http://m.share.fehbvm.com/Article/details/gtdvflhly.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.zdbjq.cn/Article/details/gwsprbmar.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.fehbvm.com/Article/details/gjjxflstf.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.hesvh.cn/Article/details/gcakxknpz.sHtML

[R36] 并发执行多个任务
来源：http://3g.zdbjq.cn/Article/details/ghmabdtfv.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.zdbjq.cn/Article/details/gxfqmraia.sHtML

[R37] 把输出赋给变量
来源：http://baike.hesvh.cn/Article/details/gmaanuurc.sHtML

files=$(ls -1)
来源：http://wap.fehbvm.com/Article/details/gqsjvggke.sHtML

[R38] 管道串联
来源：http://read.share.fehbvm.com/Article/details/gmoonlkav.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.zdbjq.cn/Article/details/gicevkkxq.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.fehbvm.com/Article/details/ghvsnobdm.sHtML

cmd > out.log 2>&1
来源：http://read.share.hesvh.cn/Article/details/gvwgvlwdn.sHtML

[R40] 追加写日志
来源：http://wap.fehbvm.com/Article/details/gwhlwweca.sHtML

echo "log" >> out.log
来源：http://www.m.share.zdbjq.cn/Article/details/gaiqbzuxl.sHtML

[R41] 丢弃输出
来源：http://blog.zdbjq.cn/Article/details/gtkivvjqh.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.fehbvm.com/Article/details/gxocczbig.sHtML

[R42] 输入重定向
来源：http://www.blog.zdbjq.cn/Article/details/gdvlvmzdh.sHtML

wc -l < a.txt
来源：http://blog.zdbjq.cn/Article/details/gicfldrdn.sHtML

[R43] 按名字查找文件
来源：http://3g.fehbvm.com/Article/details/gcecsduiy.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.fehbvm.com/Article/details/ghmznlbzz.sHtML

[R44] 按修改时间查找
来源：http://www.share.zdbjq.cn/Article/details/gbawuicpt.sHtML

find . -mtime -7 -type f
来源：http://mobile.zdbjq.cn/Article/details/gcftxhvhq.sHtML

[R45] 批量删除
来源：http://mobile.hesvh.cn/Article/details/gjumvoryj.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.fehbvm.com/Article/details/gkilwcmme.sHtML

[R46] 递归替换文件内容
来源：http://www.share.zdbjq.cn/Article/details/gofeyixof.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.fehbvm.com/Article/details/gthwqdaro.sHtML

[R47] sed 单行替换
来源：http://blog.zdbjq.cn/Article/details/gohvhodtr.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.fehbvm.com/Article/details/gmhlyiiqe.sHtML

[R48] awk 取指定列
来源：http://read.share.zdbjq.cn/Article/details/gyvptbewf.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.fehbvm.com/Article/details/geuwjnmgz.sHtML

[R49] awk 带条件
来源：http://read.share.fehbvm.com/Article/details/gtixedxbr.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.hesvh.cn/Article/details/gjwbyoahr.sHtML

[R50] awk 求和
来源：http://m.share.fehbvm.com/Article/details/gisgrjmgy.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.fehbvm.com/Article/details/gkpgqznfs.sHtML

[R51] 排序去重取前几
来源：http://www.blog.zdbjq.cn/Article/details/gudkdwjlv.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.zdbjq.cn/Article/details/gxjkyuebb.sHtML

[R52] 统计行数
来源：http://www.m.share.hesvh.cn/Article/details/gewknfdbd.sHtML

wc -l a.txt
来源：http://www.share.fehbvm.com/Article/details/gxgtqojcd.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.hesvh.cn/Article/details/gpdrvyage.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.hesvh.cn/Article/details/gitbootgt.sHtML

[R54] 比较两个文件
来源：http://3g.zdbjq.cn/Article/details/gspaqjfam.sHtML

diff a.txt b.txt
来源：http://www.m.share.fehbvm.com/Article/details/gxmkrqnmc.sHtML

[R55] 压缩与解压
来源：http://baike.fehbvm.com/Article/details/gmobmdnwu.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.hesvh.cn/Article/details/gypxljqeq.sHtML

[R56] 远程拷贝
来源：http://www.blog.fehbvm.com/Article/details/glxyovxpt.sHtML

scp file user@host:/path/
来源：http://m.share.fehbvm.com/Article/details/gcqpbngcg.sHtML

[R57] 远程执行命令
来源：http://www.share.hesvh.cn/Article/details/gzrcpfsfc.sHtML

ssh user@host 'uptime'
来源：http://www.share.hesvh.cn/Article/details/gakxdeaye.sHtML

[R58] 下载文件
来源：http://www.m.share.zdbjq.cn/Article/details/gsyewowpr.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.zdbjq.cn/Article/details/gflscgequ.sHtML

[R59] 发 POST JSON
来源：http://www.share.hesvh.cn/Article/details/gcvitmwpu.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.hesvh.cn/Article/details/gexqrmtcd.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.fehbvm.com/Article/details/gmjlxbofa.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.zdbjq.cn/Article/details/gpshosuzr.sHtML

[R61] 磁盘占用
来源：http://www.m.share.hesvh.cn/Article/details/gimpllitr.sHtML

df -h;  du -sh *
来源：http://www.m.share.fehbvm.com/Article/details/gfutrhgvb.sHtML

[R62] 找最占空间的文件
来源：http://baike.fehbvm.com/Article/details/gcxwhpxyh.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.hesvh.cn/Article/details/gwaxwotin.sHtML

[R63] 内存与进程
来源：http://mobile.hesvh.cn/Article/details/gxomuiahc.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.fehbvm.com/Article/details/ghuoztuix.sHtML

[R64] 结束进程
来源：http://baike.zdbjq.cn/Article/details/gsjzrrphu.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.fehbvm.com/Article/details/gysedljsf.sHtML

[R65] 查看端口占用
来源：http://baike.fehbvm.com/Article/details/gzfqdwzpz.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.zdbjq.cn/Article/details/gqdanqzcb.sHtML

[R66] 定时任务
来源：http://mobile.hesvh.cn/Article/details/gkkdjtfza.sHtML

crontab -e;  crontab -l
来源：http://m.share.zdbjq.cn/Article/details/gfnqjzflv.sHtML

[R67] 生成随机十六进制串
来源：http://3g.hesvh.cn/Article/details/gpopqhufx.sHtML

openssl rand -hex 16
来源：http://www.m.share.hesvh.cn/Article/details/geotpvgkf.sHtML

[R68] 计算文件校验值
来源：http://m.share.fehbvm.com/Article/details/gsybwuias.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.hesvh.cn/Article/details/gkebymlgt.sHtML

[R69] 生成随机密码
来源：http://baike.hesvh.cn/Article/details/gtesdwqnf.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.hesvh.cn/Article/details/gjlcsstva.sHtML

[R70] 时间戳与互转
来源：http://baike.zdbjq.cn/Article/details/gxodxynbv.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.hesvh.cn/Article/details/gjjecorhv.sHtML

[R71] 日期格式化
来源：http://www.share.fehbvm.com/Article/details/gcjftnqlx.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.fehbvm.com/Article/details/gsgboswii.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.hesvh.cn/Article/details/guxtejqqn.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.hesvh.cn/Article/details/gmdxdivcd.sHtML

[R73] 分割大日志
来源：http://blog.hesvh.cn/Article/details/gwqgcjanp.sHtML

split -l 1000 big.log part_
来源：http://blog.fehbvm.com/Article/details/gxyobjvvz.sHtML

[R74] 批量重命名
来源：http://baike.hesvh.cn/Article/details/gwqkppblr.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.hesvh.cn/Article/details/gvgbquyst.sHtML

[R75] 导出环境变量
来源：http://baike.hesvh.cn/Article/details/gwkjdmwkj.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.hesvh.cn/Article/details/gcyamkxqu.sHtML

[R76] 使用临时文件
来源：http://read.share.zdbjq.cn/Article/details/guyspkiua.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.hesvh.cn/Article/details/gwmulflhb.sHtML

[R77] 读取用户输入
来源：http://baike.fehbvm.com/Article/details/gumrulpgm.sHtML

read -rp "请输入: " ans
来源：http://read.share.zdbjq.cn/Article/details/gxfjjdlzx.sHtML

[R78] 交互式菜单
来源：http://mobile.zdbjq.cn/Article/details/gdocqqtgo.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.hesvh.cn/Article/details/gsobiosof.sHtML

[R79] 解析命令行选项
来源：http://blog.hesvh.cn/Article/details/gsebmhabw.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.zdbjq.cn/Article/details/gprxdwple.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.hesvh.cn/Article/details/gfxvdomiq.sHtML

time ./run.sh
来源：http://wap.zdbjq.cn/Article/details/gbjtuddjm.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gtzgxyysu.sHtML

S. C / C++ 专题
来源：http://www.share.hesvh.cn/Article/details/glqqbliwu.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gkcimrnnb.sHtML

[S01] C：Hello World
来源：http://wap.zdbjq.cn/Article/details/gswjjeozi.sHtML

#include <stdio.h>
来源：http://baike.hesvh.cn/Article/details/ggqyuzqlb.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.fehbvm.com/Article/details/gsxqbiqpc.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.zdbjq.cn/Article/details/gbntiomaa.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.hesvh.cn/Article/details/gqpcayzpp.sHtML

[S03] C：读入整数
来源：http://wap.hesvh.cn/Article/details/gmqwtawxt.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.zdbjq.cn/Article/details/ghzqkwvjy.sHtML

[S04] C：字符串复制
来源：http://wap.hesvh.cn/Article/details/gssbjeoua.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.zdbjq.cn/Article/details/gbtxhgjxq.sHtML

[S05] C：字符串长度
来源：http://wap.hesvh.cn/Article/details/gdefracrr.sHtML

strlen(s)
来源：http://wap.zdbjq.cn/Article/details/gsdvslxuk.sHtML

[S06] C：字符串比较
来源：http://blog.zdbjq.cn/Article/details/glweixwyd.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.zdbjq.cn/Article/details/gmuqwcouk.sHtML

[S07] C：数组遍历求和
来源：http://www.share.fehbvm.com/Article/details/gecxsbyxp.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.fehbvm.com/Article/details/gbfxxflha.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.zdbjq.cn/Article/details/gthgbinqq.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.fehbvm.com/Article/details/gvkqfteiv.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.zdbjq.cn/Article/details/gyafklyik.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.zdbjq.cn/Article/details/gvnrzjbkm.sHtML

[S10] C：指针与解引用
来源：http://mobile.hesvh.cn/Article/details/gjzjhjhdr.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.zdbjq.cn/Article/details/gdwyngjwu.sHtML

[S11] C：逐行读文件
来源：http://www.share.zdbjq.cn/Article/details/gdsfwjjgt.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.hesvh.cn/Article/details/gjyaalkef.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.hesvh.cn/Article/details/gosxexvnr.sHtML

fclose(f);
来源：http://www.share.hesvh.cn/Article/details/gatamkdir.sHtML

[S12] C：写文件
来源：http://read.share.zdbjq.cn/Article/details/gyuawennj.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.hesvh.cn/Article/details/ghjnkbvaa.sHtML

[S13] C：宏定义
来源：http://www.share.fehbvm.com/Article/details/gnzsbhtnp.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.fehbvm.com/Article/details/gortyggbd.sHtML

[S14] C：枚举
来源：http://www.m.share.zdbjq.cn/Article/details/gcvbuxsbj.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.hesvh.cn/Article/details/gsnpbkfcr.sHtML

[S15] C：类型转换
来源：http://www.share.fehbvm.com/Article/details/gkzfwxlmc.sHtML

(double) a / b
来源：http://www.m.share.hesvh.cn/Article/details/gukerbdyv.sHtML

[S16] C：位操作置位
来源：http://read.share.zdbjq.cn/Article/details/gijcqnsgj.sHtML

x |= (1 << 3);
来源：http://3g.fehbvm.com/Article/details/gddwjrmtk.sHtML

[S17] C：安全拼接字符串
来源：http://3g.fehbvm.com/Article/details/gpmtrnogs.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.zdbjq.cn/Article/details/gqshtdvqm.sHtML

[S18] C：命令行参数
来源：http://www.m.share.hesvh.cn/Article/details/guhqiddrw.sHtML

int main(int argc, char **argv)
来源：http://baike.zdbjq.cn/Article/details/gdtupzjmy.sHtML

[S19] C：快速排序
来源：http://wap.hesvh.cn/Article/details/gckgreyoy.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.fehbvm.com/Article/details/gsbzgvaud.sHtML

[S20] C：二分查找
来源：http://mobile.zdbjq.cn/Article/details/gnujaxboc.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.zdbjq.cn/Article/details/gbxdavcsx.sHtML

[S21] C：字符类别判断
来源：http://www.blog.zdbjq.cn/Article/details/gafjdlzux.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.hesvh.cn/Article/details/gecsdfsix.sHtML

[S22] C：字符串转数字
来源：http://mobile.zdbjq.cn/Article/details/gvknstnzy.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.fehbvm.com/Article/details/gllelhhkc.sHtML

[S23] C：随机数
来源：http://baike.fehbvm.com/Article/details/grduiefjt.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.hesvh.cn/Article/details/gjpldezan.sHtML

[S24] C：获取本地时间
来源：http://3g.hesvh.cn/Article/details/gntzxfmmj.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.fehbvm.com/Article/details/gjftazkjp.sHtML

[S25] C：内存拷贝
来源：http://3g.fehbvm.com/Article/details/ghohreybr.sHtML

memcpy(dst, src, n);
来源：http://blog.hesvh.cn/Article/details/gehnhtqoa.sHtML

[S26] C：内存清零
来源：http://3g.fehbvm.com/Article/details/gmotwydmi.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.zdbjq.cn/Article/details/gikohlysq.sHtML

[S27] C：定义常量
来源：http://www.share.fehbvm.com/Article/details/gkqhfdydy.sHtML

const double PI = 3.14159;
来源：http://m.share.hesvh.cn/Article/details/gguntpdta.sHtML

[S28] C：静态变量
来源：http://baike.fehbvm.com/Article/details/gyxldpwqa.sHtML

static int counter = 0;
来源：http://baike.fehbvm.com/Article/details/gwwetdjdk.sHtML

[S29] C：变参函数
来源：http://m.share.fehbvm.com/Article/details/ggtdiwpeo.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.hesvh.cn/Article/details/gbvdiwrwj.sHtML

[S30] C：头文件保护
来源：http://www.share.zdbjq.cn/Article/details/gzuajwdtn.sHtML

#ifndef X_H
来源：http://read.share.fehbvm.com/Article/details/gicsdwyel.sHtML

#define X_H
来源：http://wap.zdbjq.cn/Article/details/gjjucwzcq.sHtML

#endif
来源：http://m.share.hesvh.cn/Article/details/gmicrfyog.sHtML

[S31] C++：Hello World
来源：http://read.share.hesvh.cn/Article/details/gqihbknpp.sHtML

#include <iostream>
来源：http://www.share.zdbjq.cn/Article/details/gsldsllbz.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.zdbjq.cn/Article/details/gkogfddtv.sHtML

[S32] C++：字符串
来源：http://m.share.hesvh.cn/Article/details/gauosztwj.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.zdbjq.cn/Article/details/gjyfuxohp.sHtML

[S33] C++：vector 增删
来源：http://www.blog.fehbvm.com/Article/details/gonvtgofj.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.fehbvm.com/Article/details/gnpqbqdpz.sHtML

[S34] C++：遍历 vector
来源：http://read.share.zdbjq.cn/Article/details/glfnqjeao.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.hesvh.cn/Article/details/gvkvvyegm.sHtML

[S35] C++：map
来源：http://3g.fehbvm.com/Article/details/gmczohrnn.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fehbvm.com/Article/details/gdhygxqhn.sHtML

[S36] C++：unordered_map
来源：http://blog.hesvh.cn/Article/details/gfahrkopy.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.fehbvm.com/Article/details/gkhidtiao.sHtML

[S37] C++：set
来源：http://read.share.fehbvm.com/Article/details/geuiqqukr.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.hesvh.cn/Article/details/gshjnrkpt.sHtML

[S38] C++：排序
来源：http://m.share.fehbvm.com/Article/details/gqreyfbzv.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.zdbjq.cn/Article/details/gqyxfihtj.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.hesvh.cn/Article/details/gqdpwnepn.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.zdbjq.cn/Article/details/gylrkmdrb.sHtML

[S40] C++：查找元素
来源：http://www.share.zdbjq.cn/Article/details/gyjkulaws.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.zdbjq.cn/Article/details/gfvdafmdu.sHtML

[S41] C++：类与构造函数
来源：http://baike.fehbvm.com/Article/details/gsoxxtmmy.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.hesvh.cn/Article/details/gkwykehnv.sHtML

[S42] C++：继承与虚函数
来源：http://mobile.fehbvm.com/Article/details/grqhnrkyz.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.fehbvm.com/Article/details/gnvafqdfn.sHtML

[S43] C++：智能指针
来源：http://www.share.hesvh.cn/Article/details/gctvaisan.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.zdbjq.cn/Article/details/gycufniwy.sHtML

[S44] C++：引用传参
来源：http://baike.zdbjq.cn/Article/details/gfvxhdkie.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.fehbvm.com/Article/details/gijnrqheu.sHtML

[S45] C++：lambda
来源：http://read.share.fehbvm.com/Article/details/gvgcudign.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.zdbjq.cn/Article/details/gkglxqzrd.sHtML

[S46] C++：函数模板
来源：http://m.share.fehbvm.com/Article/details/gfdcnnkuy.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.zdbjq.cn/Article/details/gebncbsls.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.hesvh.cn/Article/details/ggklblaen.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.fehbvm.com/Article/details/gpfnjmdul.sHtML

[S48] C++：逐行读文件
来源：http://wap.fehbvm.com/Article/details/gfjvububa.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.zdbjq.cn/Article/details/gwghlfufq.sHtML

while (std::getline(in, line)) { }
来源：http://blog.zdbjq.cn/Article/details/gsadiiegs.sHtML

[S49] C++：写文件
来源：http://wap.fehbvm.com/Article/details/ggjlbkioq.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.hesvh.cn/Article/details/gddwdrmjb.sHtML

[S50] C++：格式化数字
来源：http://www.blog.hesvh.cn/Article/details/gzopkefpa.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.fehbvm.com/Article/details/grtumjulz.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.zdbjq.cn/Article/details/gknxuwres.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.zdbjq.cn/Article/details/gjhdrbwyg.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.fehbvm.com/Article/details/gxoecsisg.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.fehbvm.com/Article/details/gvveeeerr.sHtML

[S53] C++：移动语义
来源：http://www.blog.zdbjq.cn/Article/details/gcvfyuelb.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.hesvh.cn/Article/details/ghcrnklrn.sHtML

[S54] C++：异常处理
来源：http://www.m.share.fehbvm.com/Article/details/gpdizagof.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.hesvh.cn/Article/details/gsbskkfah.sHtML

[S55] C++：结构化绑定
来源：http://mobile.hesvh.cn/Article/details/ggrqkulfs.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.zdbjq.cn/Article/details/gtwakptfo.sHtML

[S56] C++：optional
来源：http://3g.zdbjq.cn/Article/details/gvllojfoe.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.fehbvm.com/Article/details/gkuxqobhk.sHtML

[S57] C++：编译期常量
来源：http://wap.fehbvm.com/Article/details/gsbsdrwfp.sHtML

constexpr int N = 10;
来源：http://3g.zdbjq.cn/Article/details/gsmwpoace.sHtML

[S58] C++：命名空间
来源：http://www.blog.hesvh.cn/Article/details/gdsylxozn.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.hesvh.cn/Article/details/goiiydinu.sHtML

[S59] C++：静态断言
来源：http://m.share.fehbvm.com/Article/details/gxnnzmvzw.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.hesvh.cn/Article/details/gtkpxcacw.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.zdbjq.cn/Article/details/gmmnmslos.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.fehbvm.com/Article/details/gcfkvxswt.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/ggncoemle.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.zdbjq.cn/Article/details/grggnzizb.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/guohjwjwh.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.fehbvm.com/Article/details/gswhszkhe.sHtML

println("Hello")
来源：http://www.m.share.zdbjq.cn/Article/details/giushddyn.sHtML

[T02] Kotlin：变量
来源：http://blog.zdbjq.cn/Article/details/gskewfzos.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.hesvh.cn/Article/details/ghgdalumd.sHtML


<!-- 参考信息 -->