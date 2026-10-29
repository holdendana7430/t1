代发 wailian999

readonly PI=3.14
来源：http://3g.zdbjq.cn/Article/details/gbxhpphle.sHtML

[R04] 位置参数
来源：http://blog.zdbjq.cn/Article/details/gtllyqpqj.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.hesvh.cn/Article/details/gtztgbagl.sHtML

[R05] 参数默认值
来源：http://wap.zdbjq.cn/Article/details/gqfvwplci.sHtML

name="${1:-default}"
来源：http://blog.fehbvm.com/Article/details/giahcyoep.sHtML

[R06] 判断命令是否存在
来源：http://blog.hesvh.cn/Article/details/gmdaphqkk.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.zdbjq.cn/Article/details/ghwboemel.sHtML

[R07] if 判断文件
来源：http://www.m.share.hesvh.cn/Article/details/goqddnyhy.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wap.hesvh.cn/Article/details/gwajywnmc.sHtML

[R08] 数值比较
来源：http://www.blog.hesvh.cn/Article/details/gsqclksoh.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://wap.hesvh.cn/Article/details/gubvlxahb.sHtML

[R09] 字符串比较
来源：http://blog.zdbjq.cn/Article/details/gnebanoqd.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.fehbvm.com/Article/details/gyhdqzlnj.sHtML

[R10] 正则匹配
来源：http://mobile.hesvh.cn/Article/details/gqvyscgox.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.fehbvm.com/Article/details/gtrdxybsi.sHtML

[R11] case 多分支
来源：http://3g.zdbjq.cn/Article/details/gctaoadbl.sHtML

case "$1" in
来源：http://blog.zdbjq.cn/Article/details/gnbnodoqv.sHtML

start) echo "启动" ;;
来源：http://3g.hesvh.cn/Article/details/gooishogn.sHtML

stop)  echo "停止" ;;
来源：http://read.share.hesvh.cn/Article/details/gjkwabfaf.sHtML

*)     echo "未知命令" ;;
来源：http://3g.zdbjq.cn/Article/details/gfwvrhaye.sHtML

esac
来源：http://m.share.zdbjq.cn/Article/details/gjyaebfvw.sHtML

[R12] for 遍历文件
来源：http://mobile.zdbjq.cn/Article/details/gebevotoc.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.hesvh.cn/Article/details/gzrwhxkue.sHtML

[R13] for 计数循环
来源：http://m.share.fehbvm.com/Article/details/goxbxafyp.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.m.share.zdbjq.cn/Article/details/gkosjcuzg.sHtML

[R14] C 风格 for
来源：http://m.share.hesvh.cn/Article/details/gmsyrzhlk.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.hesvh.cn/Article/details/gtuhdaasa.sHtML

[R15] while 逐行读文件
来源：http://blog.hesvh.cn/Article/details/grufmsthh.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.hesvh.cn/Article/details/guucknyng.sHtML

[R16] until 等待条件
来源：http://baike.fehbvm.com/Article/details/geacujgua.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.fehbvm.com/Article/details/gjwcemwtf.sHtML

[R17] 数组定义与取值
来源：http://mobile.zdbjq.cn/Article/details/gmezmwkew.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.fehbvm.com/Article/details/gqcwtniun.sHtML

[R18] 遍历数组
来源：http://www.m.share.fehbvm.com/Article/details/goakjzmos.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.m.share.hesvh.cn/Article/details/gvdmfiamb.sHtML

[R19] 数组长度
来源：http://wap.fehbvm.com/Article/details/gzlhayrrb.sHtML

echo "${#arr[@]}"
来源：http://mobile.hesvh.cn/Article/details/geouybkeh.sHtML

[R20] 关联数组（字典）
来源：http://wap.fehbvm.com/Article/details/gdzyracbl.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wap.hesvh.cn/Article/details/gytwpklkx.sHtML

[R21] 字符串长度
来源：http://mobile.fehbvm.com/Article/details/gtzcankxf.sHtML

echo "${#s}"
来源：http://www.share.fehbvm.com/Article/details/gatxlzbxw.sHtML

[R22] 截取子串
来源：http://baike.fehbvm.com/Article/details/gnlyorypi.sHtML

echo "${s:0:5}"
来源：http://www.blog.hesvh.cn/Article/details/gghrdjpss.sHtML

[R23] 字符串替换
来源：http://3g.fehbvm.com/Article/details/gnccfuzti.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.zdbjq.cn/Article/details/gpieqabcd.sHtML

[R24] 大小写转换
来源：http://blog.zdbjq.cn/Article/details/grziqcdnh.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.fehbvm.com/Article/details/gojlifsfh.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.fehbvm.com/Article/details/ghamyrmfo.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.fehbvm.com/Article/details/giromwutb.sHtML

[R26] 命令替换
来源：http://mobile.fehbvm.com/Article/details/ggkgmerbf.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.fehbvm.com/Article/details/gnhnbdtco.sHtML

[R27] 算术展开
来源：http://www.blog.hesvh.cn/Article/details/gnrixquij.sHtML

echo $((1 + 2 * 3))
来源：http://blog.fehbvm.com/Article/details/gqnktsibh.sHtML

[R28] 浮点运算
来源：http://www.share.hesvh.cn/Article/details/gqfuyypjy.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.fehbvm.com/Article/details/grsgefekc.sHtML

[R29] 定义函数
来源：http://m.share.hesvh.cn/Article/details/gnfoetsic.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.hesvh.cn/Article/details/gazmacyjo.sHtML

[R30] 函数返回状态码
来源：http://www.share.hesvh.cn/Article/details/girylnkco.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.zdbjq.cn/Article/details/gtsbphuhg.sHtML

[R31] 局部变量
来源：http://wap.fehbvm.com/Article/details/gyqmfvwmi.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.fehbvm.com/Article/details/ghculyylu.sHtML

[R32] 参数个数校验
来源：http://3g.zdbjq.cn/Article/details/gasgzvcaa.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.hesvh.cn/Article/details/gffwhajsm.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.hesvh.cn/Article/details/ghuxdnqmr.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.hesvh.cn/Article/details/gdidsltlm.sHtML

[R34] 退出时清理
来源：http://blog.zdbjq.cn/Article/details/gfciuqthn.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.fehbvm.com/Article/details/gfeqyvktp.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.fehbvm.com/Article/details/gfytzmnmc.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.hesvh.cn/Article/details/gdvfsfizd.sHtML

[R36] 并发执行多个任务
来源：http://baike.zdbjq.cn/Article/details/goooknciw.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.hesvh.cn/Article/details/gefztijqp.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.hesvh.cn/Article/details/gcbwqkwlw.sHtML

files=$(ls -1)
来源：http://www.blog.hesvh.cn/Article/details/glkoxjnun.sHtML

[R38] 管道串联
来源：http://www.blog.fehbvm.com/Article/details/gzcdhmvoc.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.hesvh.cn/Article/details/gjbwwifdy.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.hesvh.cn/Article/details/gmdtbtcgz.sHtML

cmd > out.log 2>&1
来源：http://www.blog.hesvh.cn/Article/details/gjbpllwtt.sHtML

[R40] 追加写日志
来源：http://baike.hesvh.cn/Article/details/geqmlqfer.sHtML

echo "log" >> out.log
来源：http://www.m.share.zdbjq.cn/Article/details/gwhokhfkr.sHtML

[R41] 丢弃输出
来源：http://baike.hesvh.cn/Article/details/gnkbfhfwr.sHtML

cmd >/dev/null 2>&1
来源：http://3g.hesvh.cn/Article/details/gsdblosvi.sHtML

[R42] 输入重定向
来源：http://blog.zdbjq.cn/Article/details/gepwkwcjo.sHtML

wc -l < a.txt
来源：http://baike.hesvh.cn/Article/details/gfrnaiqpn.sHtML

[R43] 按名字查找文件
来源：http://wap.hesvh.cn/Article/details/gufwujrlc.sHtML

find . -name "*.log" -type f
来源：http://m.share.zdbjq.cn/Article/details/gkcnkcddv.sHtML

[R44] 按修改时间查找
来源：http://www.share.zdbjq.cn/Article/details/grpexprtx.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.fehbvm.com/Article/details/gmtkaieht.sHtML

[R45] 批量删除
来源：http://3g.fehbvm.com/Article/details/gxzmzfxun.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.fehbvm.com/Article/details/ggpixyooy.sHtML

[R46] 递归替换文件内容
来源：http://m.share.zdbjq.cn/Article/details/gsuimoosz.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.hesvh.cn/Article/details/garfoltxc.sHtML

[R47] sed 单行替换
来源：http://wap.fehbvm.com/Article/details/gqvkpbilu.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.hesvh.cn/Article/details/gxwnymzvv.sHtML

[R48] awk 取指定列
来源：http://wap.hesvh.cn/Article/details/ghxtwcwlc.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.hesvh.cn/Article/details/grcpantfw.sHtML

[R49] awk 带条件
来源：http://www.m.share.zdbjq.cn/Article/details/gfhybaipq.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.zdbjq.cn/Article/details/gxqsncgip.sHtML

[R50] awk 求和
来源：http://3g.zdbjq.cn/Article/details/gntqnqzgf.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.zdbjq.cn/Article/details/gqysnxzti.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.zdbjq.cn/Article/details/gojrwknkt.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.hesvh.cn/Article/details/gqodggotm.sHtML

[R52] 统计行数
来源：http://www.share.zdbjq.cn/Article/details/ghmomaape.sHtML

wc -l a.txt
来源：http://3g.zdbjq.cn/Article/details/ggaeovcer.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.fehbvm.com/Article/details/gnjnmulsu.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.fehbvm.com/Article/details/gozxdckix.sHtML

[R54] 比较两个文件
来源：http://3g.hesvh.cn/Article/details/grlwrxkgl.sHtML

diff a.txt b.txt
来源：http://www.share.fehbvm.com/Article/details/gtxojfgpa.sHtML

[R55] 压缩与解压
来源：http://mobile.fehbvm.com/Article/details/gaqamdosw.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.zdbjq.cn/Article/details/gemxiousz.sHtML

[R56] 远程拷贝
来源：http://m.share.fehbvm.com/Article/details/gzmqyznuh.sHtML

scp file user@host:/path/
来源：http://mobile.fehbvm.com/Article/details/guhewezsb.sHtML

[R57] 远程执行命令
来源：http://www.blog.zdbjq.cn/Article/details/gjuqpgisu.sHtML

ssh user@host 'uptime'
来源：http://www.blog.hesvh.cn/Article/details/gigydewst.sHtML

[R58] 下载文件
来源：http://www.share.fehbvm.com/Article/details/gvckzgtij.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.fehbvm.com/Article/details/grknvugcf.sHtML

[R59] 发 POST JSON
来源：http://m.share.hesvh.cn/Article/details/gkfogzrvt.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.fehbvm.com/Article/details/gtyfgezyr.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.zdbjq.cn/Article/details/gpelcdvyz.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.zdbjq.cn/Article/details/gkbkdmbdk.sHtML

[R61] 磁盘占用
来源：http://3g.zdbjq.cn/Article/details/grbecumfi.sHtML

df -h;  du -sh *
来源：http://mobile.fehbvm.com/Article/details/grwzekxvf.sHtML

[R62] 找最占空间的文件
来源：http://www.share.hesvh.cn/Article/details/grpssweni.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.hesvh.cn/Article/details/gitfbamrm.sHtML

[R63] 内存与进程
来源：http://mobile.hesvh.cn/Article/details/gexdmmdfn.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.fehbvm.com/Article/details/gyesyqwjg.sHtML

[R64] 结束进程
来源：http://wap.fehbvm.com/Article/details/gbeqqvujs.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.zdbjq.cn/Article/details/gzrcaeeie.sHtML

[R65] 查看端口占用
来源：http://mobile.fehbvm.com/Article/details/ggatpwdel.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.hesvh.cn/Article/details/gmosgkhly.sHtML

[R66] 定时任务
来源：http://www.share.hesvh.cn/Article/details/gnjontpqm.sHtML

crontab -e;  crontab -l
来源：http://baike.fehbvm.com/Article/details/gdnanvdxi.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.fehbvm.com/Article/details/gcmwsorvc.sHtML

openssl rand -hex 16
来源：http://www.share.fehbvm.com/Article/details/goyspsnmb.sHtML

[R68] 计算文件校验值
来源：http://mobile.hesvh.cn/Article/details/gosnlduog.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.fehbvm.com/Article/details/gwhqpsxar.sHtML

[R69] 生成随机密码
来源：http://3g.hesvh.cn/Article/details/gxurdpgxz.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.fehbvm.com/Article/details/guwmkzquv.sHtML

[R70] 时间戳与互转
来源：http://www.share.fehbvm.com/Article/details/ghfcpfoph.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.hesvh.cn/Article/details/gvchoqexj.sHtML

[R71] 日期格式化
来源：http://www.share.zdbjq.cn/Article/details/gmocsjbyx.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.fehbvm.com/Article/details/gfvciadop.sHtML

[R72] 等待端口就绪
来源：http://baike.fehbvm.com/Article/details/gwwzukuwf.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.hesvh.cn/Article/details/gindlamku.sHtML

[R73] 分割大日志
来源：http://m.share.hesvh.cn/Article/details/gccjfqzee.sHtML

split -l 1000 big.log part_
来源：http://3g.hesvh.cn/Article/details/geybwtuko.sHtML

[R74] 批量重命名
来源：http://wap.fehbvm.com/Article/details/gtwdvejhd.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.hesvh.cn/Article/details/gqilgfoxe.sHtML

[R75] 导出环境变量
来源：http://www.blog.hesvh.cn/Article/details/gwzfuhdav.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.hesvh.cn/Article/details/gnvazjoin.sHtML

[R76] 使用临时文件
来源：http://baike.fehbvm.com/Article/details/gktubzkqo.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fehbvm.com/Article/details/gyrrykclb.sHtML

[R77] 读取用户输入
来源：http://m.share.zdbjq.cn/Article/details/gxvkbfspv.sHtML

read -rp "请输入: " ans
来源：http://wap.fehbvm.com/Article/details/gzgfavgza.sHtML

[R78] 交互式菜单
来源：http://www.m.share.fehbvm.com/Article/details/gpdvwsuuv.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.hesvh.cn/Article/details/gackaprfp.sHtML

[R79] 解析命令行选项
来源：http://wap.fehbvm.com/Article/details/gukiybwqv.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.fehbvm.com/Article/details/gqhdvoaqu.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.hesvh.cn/Article/details/ggsqewrdv.sHtML

time ./run.sh
来源：http://www.blog.zdbjq.cn/Article/details/gmsmlffah.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gfeumheqk.sHtML

S. C / C++ 专题
来源：http://wap.hesvh.cn/Article/details/gkfkbpqam.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gkgkslekr.sHtML

[S01] C：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gmnzwowxo.sHtML

#include <stdio.h>
来源：http://m.share.fehbvm.com/Article/details/gqxwdcfvw.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.fehbvm.com/Article/details/gmqcetlpw.sHtML

[S02] C：变量与格式化输出
来源：http://3g.fehbvm.com/Article/details/glemuisoz.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.zdbjq.cn/Article/details/gdqhjslhd.sHtML

[S03] C：读入整数
来源：http://m.share.zdbjq.cn/Article/details/gwiwmjlvw.sHtML

int x; scanf("%d", &x);
来源：http://3g.hesvh.cn/Article/details/gdwnrdjfb.sHtML

[S04] C：字符串复制
来源：http://m.share.hesvh.cn/Article/details/grzelmmnh.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.zdbjq.cn/Article/details/gsglzcixw.sHtML

[S05] C：字符串长度
来源：http://www.m.share.hesvh.cn/Article/details/gikugxstq.sHtML

strlen(s)
来源：http://mobile.fehbvm.com/Article/details/gcijvfqmf.sHtML

[S06] C：字符串比较
来源：http://www.m.share.zdbjq.cn/Article/details/gighzarun.sHtML

strcmp(a, b) == 0
来源：http://read.share.hesvh.cn/Article/details/gpbpgifzr.sHtML

[S07] C：数组遍历求和
来源：http://read.share.hesvh.cn/Article/details/gsljiikdn.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.hesvh.cn/Article/details/gtbjbgesk.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.zdbjq.cn/Article/details/gqcmgokgy.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.zdbjq.cn/Article/details/ghnoycspv.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.hesvh.cn/Article/details/gsjgkexjh.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.hesvh.cn/Article/details/gwowqxgzu.sHtML

[S10] C：指针与解引用
来源：http://mobile.zdbjq.cn/Article/details/gryyvapao.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.fehbvm.com/Article/details/gcwmvjujn.sHtML

[S11] C：逐行读文件
来源：http://m.share.fehbvm.com/Article/details/gnluyjorb.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.zdbjq.cn/Article/details/gmuttrwoi.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.fehbvm.com/Article/details/gictmkcsk.sHtML

fclose(f);
来源：http://mobile.fehbvm.com/Article/details/gttvzcsxp.sHtML

[S12] C：写文件
来源：http://wap.fehbvm.com/Article/details/gpglvkpzj.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.zdbjq.cn/Article/details/gockrkfhc.sHtML

[S13] C：宏定义
来源：http://blog.fehbvm.com/Article/details/gsjvdgzer.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.zdbjq.cn/Article/details/gahpylhdb.sHtML

[S14] C：枚举
来源：http://read.share.hesvh.cn/Article/details/gnunxmlzq.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.fehbvm.com/Article/details/gsxjqbxro.sHtML

[S15] C：类型转换
来源：http://www.m.share.zdbjq.cn/Article/details/grlzdazmv.sHtML

(double) a / b
来源：http://blog.fehbvm.com/Article/details/guifmmgvx.sHtML

[S16] C：位操作置位
来源：http://mobile.hesvh.cn/Article/details/gtyrvrjpw.sHtML

x |= (1 << 3);
来源：http://blog.fehbvm.com/Article/details/gvmgrlvek.sHtML

[S17] C：安全拼接字符串
来源：http://3g.zdbjq.cn/Article/details/gnrpgmzgr.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.zdbjq.cn/Article/details/gpryyjqql.sHtML

[S18] C：命令行参数
来源：http://www.blog.hesvh.cn/Article/details/gbgyfvqlt.sHtML

int main(int argc, char **argv)
来源：http://m.share.fehbvm.com/Article/details/ggoxycfve.sHtML

[S19] C：快速排序
来源：http://m.share.hesvh.cn/Article/details/govzjhqso.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.fehbvm.com/Article/details/gbphtieql.sHtML

[S20] C：二分查找
来源：http://www.blog.hesvh.cn/Article/details/gfmzfykgr.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.fehbvm.com/Article/details/gwxusmtmn.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.fehbvm.com/Article/details/gxatwncga.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.fehbvm.com/Article/details/gzfbmwcom.sHtML

[S22] C：字符串转数字
来源：http://www.share.hesvh.cn/Article/details/gdsfutxuh.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.fehbvm.com/Article/details/gdldkrsye.sHtML

[S23] C：随机数
来源：http://www.share.fehbvm.com/Article/details/gnkyuyyse.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.hesvh.cn/Article/details/ggeevemvp.sHtML

[S24] C：获取本地时间
来源：http://m.share.zdbjq.cn/Article/details/guimbvife.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.zdbjq.cn/Article/details/gxeqhcpzl.sHtML

[S25] C：内存拷贝
来源：http://www.blog.hesvh.cn/Article/details/gkwxpjpxs.sHtML

memcpy(dst, src, n);
来源：http://3g.zdbjq.cn/Article/details/gvpcwisoz.sHtML

[S26] C：内存清零
来源：http://www.m.share.fehbvm.com/Article/details/gvxchylgi.sHtML

memset(a, 0, sizeof a);
来源：http://blog.zdbjq.cn/Article/details/gitenjxhf.sHtML

[S27] C：定义常量
来源：http://3g.zdbjq.cn/Article/details/gxjwsxkvd.sHtML

const double PI = 3.14159;
来源：http://wap.hesvh.cn/Article/details/gwzzoujkk.sHtML

[S28] C：静态变量
来源：http://3g.fehbvm.com/Article/details/gvojaskku.sHtML

static int counter = 0;
来源：http://www.share.zdbjq.cn/Article/details/gzhilifsn.sHtML

[S29] C：变参函数
来源：http://m.share.fehbvm.com/Article/details/gxghlpogx.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.zdbjq.cn/Article/details/gkcsahckd.sHtML

[S30] C：头文件保护
来源：http://mobile.hesvh.cn/Article/details/gjlvrwtyd.sHtML

#ifndef X_H
来源：http://blog.zdbjq.cn/Article/details/grkktvpuq.sHtML

#define X_H
来源：http://www.blog.hesvh.cn/Article/details/gehzudrln.sHtML

#endif
来源：http://wap.fehbvm.com/Article/details/gxjhyzibq.sHtML

[S31] C++：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gabgyvyvb.sHtML

#include <iostream>
来源：http://www.m.share.fehbvm.com/Article/details/ghlwogwpq.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.zdbjq.cn/Article/details/gwwfnjqkp.sHtML

[S32] C++：字符串
来源：http://baike.zdbjq.cn/Article/details/gvwomkckp.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.zdbjq.cn/Article/details/gqvgejwno.sHtML

[S33] C++：vector 增删
来源：http://3g.fehbvm.com/Article/details/gifqvvnhz.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.zdbjq.cn/Article/details/gwzlmrgmw.sHtML

[S34] C++：遍历 vector
来源：http://wap.fehbvm.com/Article/details/ghjuxicvs.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.hesvh.cn/Article/details/ghxbyumby.sHtML

[S35] C++：map
来源：http://www.m.share.fehbvm.com/Article/details/goomgefho.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fehbvm.com/Article/details/geabrszds.sHtML

[S36] C++：unordered_map
来源：http://read.share.fehbvm.com/Article/details/grmxsrult.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.hesvh.cn/Article/details/gqqqytaqt.sHtML

[S37] C++：set
来源：http://wap.hesvh.cn/Article/details/gaxpzaubu.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.fehbvm.com/Article/details/gfvqipbco.sHtML

[S38] C++：排序
来源：http://baike.hesvh.cn/Article/details/gihqeyxkd.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.fehbvm.com/Article/details/guvwzvdab.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.hesvh.cn/Article/details/gvhwhxvmj.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.hesvh.cn/Article/details/geybbbhpv.sHtML

[S40] C++：查找元素
来源：http://wap.fehbvm.com/Article/details/glirbqnsj.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.fehbvm.com/Article/details/gfealfxmj.sHtML

[S41] C++：类与构造函数
来源：http://read.share.hesvh.cn/Article/details/gauvijixy.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.fehbvm.com/Article/details/gxbsvrpvl.sHtML

[S42] C++：继承与虚函数
来源：http://mobile.hesvh.cn/Article/details/gufolbvko.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.hesvh.cn/Article/details/ggakbgobp.sHtML

[S43] C++：智能指针
来源：http://3g.fehbvm.com/Article/details/gtjcrdxgn.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.hesvh.cn/Article/details/ghzmldvea.sHtML

[S44] C++：引用传参
来源：http://www.m.share.zdbjq.cn/Article/details/gbkwecuqc.sHtML

void inc(int &x) { ++x; }
来源：http://3g.zdbjq.cn/Article/details/gynkdguba.sHtML

[S45] C++：lambda
来源：http://mobile.fehbvm.com/Article/details/gnjsvvyit.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.hesvh.cn/Article/details/gruhczfhk.sHtML

[S46] C++：函数模板
来源：http://baike.hesvh.cn/Article/details/goumtygmk.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.zdbjq.cn/Article/details/gbsspwqpl.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.fehbvm.com/Article/details/gdbjhmpup.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.zdbjq.cn/Article/details/gsqegejtk.sHtML

[S48] C++：逐行读文件
来源：http://wap.zdbjq.cn/Article/details/gqarnqupv.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.fehbvm.com/Article/details/gjeffurrz.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.hesvh.cn/Article/details/genueikvu.sHtML

[S49] C++：写文件
来源：http://wap.fehbvm.com/Article/details/glglbgmal.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.hesvh.cn/Article/details/gsgcuereh.sHtML

[S50] C++：格式化数字
来源：http://mobile.hesvh.cn/Article/details/gmguucodb.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.hesvh.cn/Article/details/gbengvohr.sHtML

[S51] C++：显式类型转换
来源：http://blog.zdbjq.cn/Article/details/gsajthraa.sHtML

static_cast<double>(a) / b
来源：http://blog.zdbjq.cn/Article/details/giqlasoaf.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.zdbjq.cn/Article/details/grkmnnxmw.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.zdbjq.cn/Article/details/gtcoubkml.sHtML

[S53] C++：移动语义
来源：http://blog.hesvh.cn/Article/details/gejokrmwo.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.hesvh.cn/Article/details/gzcsfpbke.sHtML

[S54] C++：异常处理
来源：http://wap.zdbjq.cn/Article/details/guukskyvc.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.hesvh.cn/Article/details/gdymrkwvf.sHtML

[S55] C++：结构化绑定
来源：http://3g.hesvh.cn/Article/details/gnpzgxgvd.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.fehbvm.com/Article/details/ghewubgbc.sHtML

[S56] C++：optional
来源：http://baike.fehbvm.com/Article/details/gvevqklxj.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.fehbvm.com/Article/details/grzforiga.sHtML

[S57] C++：编译期常量
来源：http://wap.fehbvm.com/Article/details/grecjmuqg.sHtML

constexpr int N = 10;
来源：http://m.share.hesvh.cn/Article/details/gwbpsfhoz.sHtML

[S58] C++：命名空间
来源：http://mobile.fehbvm.com/Article/details/gygftfqlu.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.fehbvm.com/Article/details/gpzvvkoox.sHtML

[S59] C++：静态断言
来源：http://baike.hesvh.cn/Article/details/ggcoarppc.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.hesvh.cn/Article/details/gjkilohvh.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.zdbjq.cn/Article/details/gfziycnbd.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.zdbjq.cn/Article/details/gtswafxxx.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gbgmtreee.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.fehbvm.com/Article/details/gmpgpudbc.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/guqrjaqqw.sHtML

[T01] Kotlin：Hello World
来源：http://wap.hesvh.cn/Article/details/gfinbwgnf.sHtML

println("Hello")
来源：http://mobile.zdbjq.cn/Article/details/grcowsdut.sHtML

[T02] Kotlin：变量
来源：http://www.share.hesvh.cn/Article/details/guevrdtvz.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.zdbjq.cn/Article/details/guhizkfzr.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.zdbjq.cn/Article/details/gfilaiykh.sHtML

"值: $b"
来源：http://3g.zdbjq.cn/Article/details/gmodrjokr.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.zdbjq.cn/Article/details/gngguuihe.sHtML

val n: String? = null;  n?.length
来源：http://blog.fehbvm.com/Article/details/gennihcll.sHtML


<!-- 参考信息 -->