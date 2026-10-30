代发 wailian999

name="${1:-default}"
来源：http://blog.hesvh.cn/Article/details/ghzzwweua.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.zdbjq.cn/Article/details/gjhqyhgxs.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.m.share.fehbvm.com/Article/details/gzomwwmpq.sHtML

[R07] if 判断文件
来源：http://baike.fehbvm.com/Article/details/gtamswcwe.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.zdbjq.cn/Article/details/gzmonsxeh.sHtML

[R08] 数值比较
来源：http://3g.fehbvm.com/Article/details/gammjqnyf.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://m.share.fehbvm.com/Article/details/gwacpyxsg.sHtML

[R09] 字符串比较
来源：http://www.blog.fehbvm.com/Article/details/gfyfvqiay.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.hesvh.cn/Article/details/gzndjroiw.sHtML

[R10] 正则匹配
来源：http://www.m.share.zdbjq.cn/Article/details/gkxsakybn.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.hesvh.cn/Article/details/gtepvtuug.sHtML

[R11] case 多分支
来源：http://3g.fehbvm.com/Article/details/glebytesx.sHtML

case "$1" in
来源：http://m.share.zdbjq.cn/Article/details/gbvxapkcg.sHtML

start) echo "启动" ;;
来源：http://wap.zdbjq.cn/Article/details/ghnhtxtas.sHtML

stop)  echo "停止" ;;
来源：http://read.share.fehbvm.com/Article/details/gnewylcdb.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.fehbvm.com/Article/details/geqzlqtop.sHtML

esac
来源：http://www.m.share.hesvh.cn/Article/details/gpdprvgec.sHtML

[R12] for 遍历文件
来源：http://m.share.zdbjq.cn/Article/details/gprbusdyv.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.zdbjq.cn/Article/details/gvddigcxz.sHtML

[R13] for 计数循环
来源：http://baike.zdbjq.cn/Article/details/gapdukpms.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.m.share.zdbjq.cn/Article/details/ghvxxtzqo.sHtML

[R14] C 风格 for
来源：http://www.share.hesvh.cn/Article/details/gsoqhpged.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.hesvh.cn/Article/details/gkfavgaxb.sHtML

[R15] while 逐行读文件
来源：http://blog.hesvh.cn/Article/details/gqnxuhlgy.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.zdbjq.cn/Article/details/gyzkcmmza.sHtML

[R16] until 等待条件
来源：http://blog.zdbjq.cn/Article/details/gdaomiuio.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.fehbvm.com/Article/details/gbccnjqnt.sHtML

[R17] 数组定义与取值
来源：http://blog.hesvh.cn/Article/details/gcqvzxtoq.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.fehbvm.com/Article/details/gcwnxhffw.sHtML

[R18] 遍历数组
来源：http://3g.fehbvm.com/Article/details/gnbpsowcz.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.fehbvm.com/Article/details/gteimbwed.sHtML

[R19] 数组长度
来源：http://3g.hesvh.cn/Article/details/gnjahoowb.sHtML

echo "${#arr[@]}"
来源：http://www.share.hesvh.cn/Article/details/gdufaqzub.sHtML

[R20] 关联数组（字典）
来源：http://wap.fehbvm.com/Article/details/gcxixhaxh.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.fehbvm.com/Article/details/gyybxiqks.sHtML

[R21] 字符串长度
来源：http://www.blog.hesvh.cn/Article/details/gujvgitrq.sHtML

echo "${#s}"
来源：http://blog.zdbjq.cn/Article/details/gcvwomsuc.sHtML

[R22] 截取子串
来源：http://www.blog.fehbvm.com/Article/details/gcoqwowac.sHtML

echo "${s:0:5}"
来源：http://www.m.share.fehbvm.com/Article/details/gwguscmyg.sHtML

[R23] 字符串替换
来源：http://baike.hesvh.cn/Article/details/gcogrjcjh.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.zdbjq.cn/Article/details/gwddqiysf.sHtML

[R24] 大小写转换
来源：http://read.share.fehbvm.com/Article/details/gnfyowjko.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.fehbvm.com/Article/details/gtavvfskf.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.hesvh.cn/Article/details/gpoemwnmf.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://read.share.hesvh.cn/Article/details/gwvtabfas.sHtML

[R26] 命令替换
来源：http://baike.fehbvm.com/Article/details/gbfjoastn.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.zdbjq.cn/Article/details/gsfaywlsd.sHtML

[R27] 算术展开
来源：http://mobile.zdbjq.cn/Article/details/ghixstswi.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.hesvh.cn/Article/details/grfxuwjdb.sHtML

[R28] 浮点运算
来源：http://baike.zdbjq.cn/Article/details/gdblacxol.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.hesvh.cn/Article/details/gbkkbocwh.sHtML

[R29] 定义函数
来源：http://3g.zdbjq.cn/Article/details/gvfurodtn.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.fehbvm.com/Article/details/gucxgnbmj.sHtML

[R30] 函数返回状态码
来源：http://blog.fehbvm.com/Article/details/gvitvfjvz.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.fehbvm.com/Article/details/gatkxpivy.sHtML

[R31] 局部变量
来源：http://m.share.hesvh.cn/Article/details/gmiuhpzze.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.hesvh.cn/Article/details/gbwjnblqk.sHtML

[R32] 参数个数校验
来源：http://baike.zdbjq.cn/Article/details/gcpubvyaf.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.zdbjq.cn/Article/details/gwmfbhkzw.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.fehbvm.com/Article/details/geuxejvrh.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.zdbjq.cn/Article/details/gbmnuxxxq.sHtML

[R34] 退出时清理
来源：http://3g.hesvh.cn/Article/details/gtenlgfnd.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.share.hesvh.cn/Article/details/gbvngmulo.sHtML

[R35] 后台执行并等待
来源：http://read.share.zdbjq.cn/Article/details/gdkjzfoea.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.hesvh.cn/Article/details/gquaklsmv.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.zdbjq.cn/Article/details/ghpmqvcqg.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.zdbjq.cn/Article/details/gukaenlde.sHtML

[R37] 把输出赋给变量
来源：http://blog.hesvh.cn/Article/details/gcxvpqbhf.sHtML

files=$(ls -1)
来源：http://www.share.zdbjq.cn/Article/details/giigawffp.sHtML

[R38] 管道串联
来源：http://baike.hesvh.cn/Article/details/glpuvjsyk.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.zdbjq.cn/Article/details/gvsqqkmrl.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.hesvh.cn/Article/details/gvsssvytf.sHtML

cmd > out.log 2>&1
来源：http://wap.hesvh.cn/Article/details/gmhrwnmab.sHtML

[R40] 追加写日志
来源：http://baike.hesvh.cn/Article/details/gjdavbirx.sHtML

echo "log" >> out.log
来源：http://mobile.zdbjq.cn/Article/details/gpzythbay.sHtML

[R41] 丢弃输出
来源：http://www.m.share.zdbjq.cn/Article/details/gunrzbxjn.sHtML

cmd >/dev/null 2>&1
来源：http://3g.hesvh.cn/Article/details/gtwaxhowv.sHtML

[R42] 输入重定向
来源：http://www.m.share.zdbjq.cn/Article/details/gwodnitwc.sHtML

wc -l < a.txt
来源：http://m.share.hesvh.cn/Article/details/gvgrlfbeq.sHtML

[R43] 按名字查找文件
来源：http://www.blog.zdbjq.cn/Article/details/gsvyvknck.sHtML

find . -name "*.log" -type f
来源：http://www.blog.fehbvm.com/Article/details/gkvsnwuvx.sHtML

[R44] 按修改时间查找
来源：http://baike.fehbvm.com/Article/details/ghntcvjbd.sHtML

find . -mtime -7 -type f
来源：http://wap.zdbjq.cn/Article/details/gfwfcfjvl.sHtML

[R45] 批量删除
来源：http://3g.hesvh.cn/Article/details/gyxdbmyfo.sHtML

find . -name "*.tmp" -delete
来源：http://wap.fehbvm.com/Article/details/gmjnnwmrh.sHtML

[R46] 递归替换文件内容
来源：http://mobile.hesvh.cn/Article/details/gtalwgxyo.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.hesvh.cn/Article/details/gqcddrcdj.sHtML

[R47] sed 单行替换
来源：http://read.share.zdbjq.cn/Article/details/ghwqpljlf.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.hesvh.cn/Article/details/gzasykams.sHtML

[R48] awk 取指定列
来源：http://m.share.hesvh.cn/Article/details/gdezribzu.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.hesvh.cn/Article/details/gtcmitplz.sHtML

[R49] awk 带条件
来源：http://baike.hesvh.cn/Article/details/gcqvwvfdq.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.zdbjq.cn/Article/details/gprrbwznv.sHtML

[R50] awk 求和
来源：http://baike.zdbjq.cn/Article/details/gcanrwzxs.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.zdbjq.cn/Article/details/gwwrawfyu.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.hesvh.cn/Article/details/gltxybvaq.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.zdbjq.cn/Article/details/gcuezhffa.sHtML

[R52] 统计行数
来源：http://baike.hesvh.cn/Article/details/gbbpnqiqs.sHtML

wc -l a.txt
来源：http://baike.zdbjq.cn/Article/details/ghfiwtkwn.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.zdbjq.cn/Article/details/gqpjvvctx.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.fehbvm.com/Article/details/guchiimat.sHtML

[R54] 比较两个文件
来源：http://www.share.fehbvm.com/Article/details/gejighkvf.sHtML

diff a.txt b.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gmsvepckr.sHtML

[R55] 压缩与解压
来源：http://3g.fehbvm.com/Article/details/gbvpthgtw.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.zdbjq.cn/Article/details/glqwlzafm.sHtML

[R56] 远程拷贝
来源：http://baike.fehbvm.com/Article/details/gsvjhwrks.sHtML

scp file user@host:/path/
来源：http://www.blog.fehbvm.com/Article/details/gcxlhdath.sHtML

[R57] 远程执行命令
来源：http://wap.zdbjq.cn/Article/details/gvtvferny.sHtML

ssh user@host 'uptime'
来源：http://www.blog.zdbjq.cn/Article/details/gawarnjqo.sHtML

[R58] 下载文件
来源：http://www.blog.fehbvm.com/Article/details/gfjacmhfu.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.fehbvm.com/Article/details/gcpuivrdf.sHtML

[R59] 发 POST JSON
来源：http://wap.fehbvm.com/Article/details/gbrxdudtp.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.zdbjq.cn/Article/details/gtarixfod.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.zdbjq.cn/Article/details/gwxcakgxv.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.fehbvm.com/Article/details/gdxbrigpk.sHtML

[R61] 磁盘占用
来源：http://www.share.fehbvm.com/Article/details/gknvxussc.sHtML

df -h;  du -sh *
来源：http://mobile.hesvh.cn/Article/details/gbnsrypfw.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.zdbjq.cn/Article/details/gbjodowqp.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.hesvh.cn/Article/details/gfqtucpqk.sHtML

[R63] 内存与进程
来源：http://3g.zdbjq.cn/Article/details/gikspaycu.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.zdbjq.cn/Article/details/gsfgbdocl.sHtML

[R64] 结束进程
来源：http://3g.fehbvm.com/Article/details/gggfvrzfk.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.hesvh.cn/Article/details/gndpneeqf.sHtML

[R65] 查看端口占用
来源：http://wap.zdbjq.cn/Article/details/ghmdgzwlm.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.fehbvm.com/Article/details/gjatcxiex.sHtML

[R66] 定时任务
来源：http://www.m.share.fehbvm.com/Article/details/gbomyzgbi.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.zdbjq.cn/Article/details/gohpzwonh.sHtML

[R67] 生成随机十六进制串
来源：http://wap.hesvh.cn/Article/details/gghkrmqxq.sHtML

openssl rand -hex 16
来源：http://wap.zdbjq.cn/Article/details/gesluiwws.sHtML

[R68] 计算文件校验值
来源：http://mobile.fehbvm.com/Article/details/gzwxnzqgk.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.zdbjq.cn/Article/details/gidfduxkg.sHtML

[R69] 生成随机密码
来源：http://3g.zdbjq.cn/Article/details/gfmfjnccx.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.zdbjq.cn/Article/details/gbcyccffw.sHtML

[R70] 时间戳与互转
来源：http://baike.fehbvm.com/Article/details/gejhrkthr.sHtML

date +%s;  date -d @1700000000
来源：http://blog.fehbvm.com/Article/details/gjanskpns.sHtML

[R71] 日期格式化
来源：http://www.m.share.fehbvm.com/Article/details/gsnuimozz.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.hesvh.cn/Article/details/gwyuqpqkl.sHtML

[R72] 等待端口就绪
来源：http://www.blog.fehbvm.com/Article/details/gayapkpzs.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.hesvh.cn/Article/details/gmlorhqtt.sHtML

[R73] 分割大日志
来源：http://www.blog.zdbjq.cn/Article/details/gajvuxfwe.sHtML

split -l 1000 big.log part_
来源：http://www.share.hesvh.cn/Article/details/gqlbutjya.sHtML

[R74] 批量重命名
来源：http://wap.fehbvm.com/Article/details/ggdlkdhxu.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.zdbjq.cn/Article/details/gciijhcsj.sHtML

[R75] 导出环境变量
来源：http://baike.zdbjq.cn/Article/details/gsucztvlw.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.hesvh.cn/Article/details/gdomocile.sHtML

[R76] 使用临时文件
来源：http://read.share.zdbjq.cn/Article/details/gdoglnrpy.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.fehbvm.com/Article/details/gjknkyykw.sHtML

[R77] 读取用户输入
来源：http://read.share.hesvh.cn/Article/details/gljgqvhkj.sHtML

read -rp "请输入: " ans
来源：http://www.blog.hesvh.cn/Article/details/ggtlvrtfd.sHtML

[R78] 交互式菜单
来源：http://mobile.hesvh.cn/Article/details/gtaodzdxo.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.fehbvm.com/Article/details/glavoyvxa.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.hesvh.cn/Article/details/gveoabguh.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.fehbvm.com/Article/details/gowuyzzsz.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.hesvh.cn/Article/details/gogfhyzsr.sHtML

time ./run.sh
来源：http://www.share.hesvh.cn/Article/details/grkbshvfd.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gnekvykdc.sHtML

S. C / C++ 专题
来源：http://blog.zdbjq.cn/Article/details/gnadfwgbh.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gwcsvshaq.sHtML

[S01] C：Hello World
来源：http://www.blog.fehbvm.com/Article/details/gkqszkpho.sHtML

#include <stdio.h>
来源：http://www.share.hesvh.cn/Article/details/gmtpwbmpy.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.fehbvm.com/Article/details/gsxzudbdk.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.fehbvm.com/Article/details/giuacqfcl.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.zdbjq.cn/Article/details/ggnlxwmiy.sHtML

[S03] C：读入整数
来源：http://www.share.fehbvm.com/Article/details/gosukphad.sHtML

int x; scanf("%d", &x);
来源：http://baike.fehbvm.com/Article/details/gzcjisbcq.sHtML

[S04] C：字符串复制
来源：http://www.blog.hesvh.cn/Article/details/gpijlamud.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.zdbjq.cn/Article/details/gdvojmwft.sHtML

[S05] C：字符串长度
来源：http://www.share.fehbvm.com/Article/details/gfrpxwfdu.sHtML

strlen(s)
来源：http://www.m.share.fehbvm.com/Article/details/givcbrdua.sHtML

[S06] C：字符串比较
来源：http://www.m.share.fehbvm.com/Article/details/gervitzgd.sHtML

strcmp(a, b) == 0
来源：http://www.blog.zdbjq.cn/Article/details/gljdcqgiz.sHtML

[S07] C：数组遍历求和
来源：http://blog.fehbvm.com/Article/details/gqgdhjvky.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.zdbjq.cn/Article/details/ggnnldfyr.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.zdbjq.cn/Article/details/gzebbkqns.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.hesvh.cn/Article/details/grintpray.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.zdbjq.cn/Article/details/gchzfknfk.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.zdbjq.cn/Article/details/gvvqxmjmf.sHtML

[S10] C：指针与解引用
来源：http://3g.fehbvm.com/Article/details/gggahmrkc.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.fehbvm.com/Article/details/gljspcrwd.sHtML

[S11] C：逐行读文件
来源：http://3g.zdbjq.cn/Article/details/ggglxxexa.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.fehbvm.com/Article/details/gqyqmergp.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.hesvh.cn/Article/details/gueyohzwy.sHtML

fclose(f);
来源：http://www.share.fehbvm.com/Article/details/gsviveysu.sHtML

[S12] C：写文件
来源：http://3g.fehbvm.com/Article/details/gfvlfsssq.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.zdbjq.cn/Article/details/gieaffrfh.sHtML

[S13] C：宏定义
来源：http://www.share.hesvh.cn/Article/details/gfskxtvnw.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.zdbjq.cn/Article/details/gaujviqrf.sHtML

[S14] C：枚举
来源：http://baike.fehbvm.com/Article/details/gtdjzirhf.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.fehbvm.com/Article/details/gwtckjfjb.sHtML

[S15] C：类型转换
来源：http://www.m.share.zdbjq.cn/Article/details/gqkhluilb.sHtML

(double) a / b
来源：http://www.blog.hesvh.cn/Article/details/gaykpdxio.sHtML

[S16] C：位操作置位
来源：http://www.blog.hesvh.cn/Article/details/gmucfohcn.sHtML

x |= (1 << 3);
来源：http://www.m.share.fehbvm.com/Article/details/gkupyurdz.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.hesvh.cn/Article/details/gsfgkzurm.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.zdbjq.cn/Article/details/gjbvygugq.sHtML

[S18] C：命令行参数
来源：http://www.blog.fehbvm.com/Article/details/gbtxoelcj.sHtML

int main(int argc, char **argv)
来源：http://m.share.hesvh.cn/Article/details/gfmbtvzss.sHtML

[S19] C：快速排序
来源：http://www.m.share.zdbjq.cn/Article/details/gqawnefvv.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.zdbjq.cn/Article/details/gjfipcowb.sHtML

[S20] C：二分查找
来源：http://www.m.share.fehbvm.com/Article/details/gwuqaspqt.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.hesvh.cn/Article/details/ggvehwjmi.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.zdbjq.cn/Article/details/guabfmvxu.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.fehbvm.com/Article/details/gkhxwlqds.sHtML

[S22] C：字符串转数字
来源：http://3g.hesvh.cn/Article/details/gnmaaxmyc.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.zdbjq.cn/Article/details/gqhvimvss.sHtML

[S23] C：随机数
来源：http://read.share.hesvh.cn/Article/details/ggmihahgc.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.fehbvm.com/Article/details/gscckfzre.sHtML

[S24] C：获取本地时间
来源：http://mobile.hesvh.cn/Article/details/gfywkpuhh.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.hesvh.cn/Article/details/gpavgkopr.sHtML

[S25] C：内存拷贝
来源：http://wap.zdbjq.cn/Article/details/gxvvctfca.sHtML

memcpy(dst, src, n);
来源：http://mobile.hesvh.cn/Article/details/ggbttqmlj.sHtML

[S26] C：内存清零
来源：http://blog.fehbvm.com/Article/details/gxagnzubt.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.fehbvm.com/Article/details/googhgzpo.sHtML

[S27] C：定义常量
来源：http://wap.hesvh.cn/Article/details/gzzwmkfyt.sHtML

const double PI = 3.14159;
来源：http://m.share.fehbvm.com/Article/details/gpuispgci.sHtML

[S28] C：静态变量
来源：http://www.blog.zdbjq.cn/Article/details/grrvoilzh.sHtML

static int counter = 0;
来源：http://www.m.share.zdbjq.cn/Article/details/gaxoryomi.sHtML

[S29] C：变参函数
来源：http://baike.zdbjq.cn/Article/details/gehmmydoq.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.hesvh.cn/Article/details/gukfvisea.sHtML

[S30] C：头文件保护
来源：http://3g.zdbjq.cn/Article/details/gbektnkgc.sHtML

#ifndef X_H
来源：http://www.blog.fehbvm.com/Article/details/gsafhltfg.sHtML

#define X_H
来源：http://www.m.share.hesvh.cn/Article/details/ggazopatu.sHtML

#endif
来源：http://www.share.zdbjq.cn/Article/details/gungzskqk.sHtML

[S31] C++：Hello World
来源：http://3g.hesvh.cn/Article/details/gbvhmzkoi.sHtML

#include <iostream>
来源：http://www.share.zdbjq.cn/Article/details/gmfjvapvc.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.zdbjq.cn/Article/details/gdtsdvzee.sHtML

[S32] C++：字符串
来源：http://m.share.zdbjq.cn/Article/details/gaemsqctc.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.hesvh.cn/Article/details/gpmjbewfv.sHtML

[S33] C++：vector 增删
来源：http://3g.fehbvm.com/Article/details/ghnxlzdyt.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.zdbjq.cn/Article/details/gvixxtsbq.sHtML

[S34] C++：遍历 vector
来源：http://m.share.fehbvm.com/Article/details/gkdrdnuav.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.zdbjq.cn/Article/details/gtlqmibzm.sHtML

[S35] C++：map
来源：http://www.share.zdbjq.cn/Article/details/gdcfcgxxk.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.zdbjq.cn/Article/details/grxlqymet.sHtML

[S36] C++：unordered_map
来源：http://read.share.hesvh.cn/Article/details/glahvalvz.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.fehbvm.com/Article/details/gaclsuyzv.sHtML

[S37] C++：set
来源：http://mobile.fehbvm.com/Article/details/gstkkoemf.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.fehbvm.com/Article/details/gwajacoyc.sHtML

[S38] C++：排序
来源：http://blog.zdbjq.cn/Article/details/gzybyygyp.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.fehbvm.com/Article/details/gvarjgleg.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.zdbjq.cn/Article/details/gfasnlpwy.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.fehbvm.com/Article/details/gwaeaawau.sHtML

[S40] C++：查找元素
来源：http://www.share.fehbvm.com/Article/details/gakfutmlj.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.fehbvm.com/Article/details/gbzmaymvr.sHtML

[S41] C++：类与构造函数
来源：http://mobile.fehbvm.com/Article/details/gzwpjxxbc.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.fehbvm.com/Article/details/gbeakmubp.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.fehbvm.com/Article/details/gkdpgypwp.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.fehbvm.com/Article/details/gnfixvpya.sHtML

[S43] C++：智能指针
来源：http://mobile.hesvh.cn/Article/details/gepudprzq.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.hesvh.cn/Article/details/gshyikohp.sHtML

[S44] C++：引用传参
来源：http://wap.fehbvm.com/Article/details/gjmvyppgq.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.hesvh.cn/Article/details/grkabmleo.sHtML

[S45] C++：lambda
来源：http://mobile.fehbvm.com/Article/details/gjfluzxbt.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.hesvh.cn/Article/details/gvwszfhyu.sHtML

[S46] C++：函数模板
来源：http://www.blog.zdbjq.cn/Article/details/gzgpfnxqa.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.hesvh.cn/Article/details/gzlkyztef.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.zdbjq.cn/Article/details/gqdhqrosw.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.zdbjq.cn/Article/details/gtciqnqqj.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.fehbvm.com/Article/details/guqsaknty.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.fehbvm.com/Article/details/gcnzocnji.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.zdbjq.cn/Article/details/gxkbarzlf.sHtML

[S49] C++：写文件
来源：http://m.share.hesvh.cn/Article/details/gbmjizeml.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.hesvh.cn/Article/details/gcgfllwze.sHtML

[S50] C++：格式化数字
来源：http://www.share.hesvh.cn/Article/details/grcbyeomq.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.zdbjq.cn/Article/details/ghtewfrbu.sHtML

[S51] C++：显式类型转换
来源：http://mobile.hesvh.cn/Article/details/gldvojqgv.sHtML

static_cast<double>(a) / b
来源：http://www.blog.zdbjq.cn/Article/details/guqqttnxv.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.hesvh.cn/Article/details/ggilezctu.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.hesvh.cn/Article/details/godrvvxxt.sHtML

[S53] C++：移动语义
来源：http://3g.hesvh.cn/Article/details/gocodnvss.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.zdbjq.cn/Article/details/gixsxcpkx.sHtML

[S54] C++：异常处理
来源：http://m.share.zdbjq.cn/Article/details/gheugauwv.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.hesvh.cn/Article/details/gydangscz.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.hesvh.cn/Article/details/gllfhuypa.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.fehbvm.com/Article/details/glhvarmhh.sHtML

[S56] C++：optional
来源：http://baike.hesvh.cn/Article/details/gomubvsfy.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.hesvh.cn/Article/details/gmxjkhmnm.sHtML

[S57] C++：编译期常量
来源：http://baike.hesvh.cn/Article/details/ggidvlwmv.sHtML

constexpr int N = 10;
来源：http://baike.hesvh.cn/Article/details/gmaeapdcl.sHtML

[S58] C++：命名空间
来源：http://blog.zdbjq.cn/Article/details/gjwuxrvfh.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.fehbvm.com/Article/details/gbcelfsgk.sHtML

[S59] C++：静态断言
来源：http://m.share.hesvh.cn/Article/details/giglbkfmb.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.zdbjq.cn/Article/details/gukbygnve.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.hesvh.cn/Article/details/gslszwrds.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.fehbvm.com/Article/details/gbaowhiyx.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gjnzwzojn.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.fehbvm.com/Article/details/gyxfwfdyr.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gphwosjzg.sHtML

[T01] Kotlin：Hello World
来源：http://3g.hesvh.cn/Article/details/gqpzblhxz.sHtML

println("Hello")
来源：http://3g.fehbvm.com/Article/details/gaksfpdiy.sHtML

[T02] Kotlin：变量
来源：http://wap.hesvh.cn/Article/details/gdxwqwcds.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.hesvh.cn/Article/details/gzkkswdhj.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.zdbjq.cn/Article/details/ghwocptbk.sHtML

"值: $b"
来源：http://3g.zdbjq.cn/Article/details/gravhvgdl.sHtML

[T04] Kotlin：空安全
来源：http://blog.hesvh.cn/Article/details/gljhtblom.sHtML

val n: String? = null;  n?.length
来源：http://m.share.zdbjq.cn/Article/details/gvmscrywa.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.fehbvm.com/Article/details/gnhdmbvzo.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.hesvh.cn/Article/details/glpbtfcpk.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.fehbvm.com/Article/details/gomspugli.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.zdbjq.cn/Article/details/graxmnoex.sHtML


<!-- 参考信息 -->