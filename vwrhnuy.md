代发 wailian999

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wap.fanxiaobao.xyz/Article/details/gphpblxcx.sHtML

[R08] 数值比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/gclsfnejc.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.fanxiaobao.xyz/Article/details/gptqlxfbi.sHtML

[R09] 字符串比较
来源：http://m.share.fanxiaobao.xyz/Article/details/gflegbfmq.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.fanxiaobao.xyz/Article/details/gnbriahlt.sHtML

[R10] 正则匹配
来源：http://blog.fanxiaobao.xyz/Article/details/ghcoejpfc.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.fanxiaobao.xyz/Article/details/gvwsajjej.sHtML

[R11] case 多分支
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbwihcnlq.sHtML

case "$1" in
来源：http://wap.fanxiaobao.xyz/Article/details/gdwueqhor.sHtML

start) echo "启动" ;;
来源：http://m.share.fanxiaobao.xyz/Article/details/gnzzuwiwh.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzvcobvro.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.fanxiaobao.xyz/Article/details/gpdtwbffj.sHtML

esac
来源：http://wap.fanxiaobao.xyz/Article/details/gxbakrjqu.sHtML

[R12] for 遍历文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gsnsysgkv.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.fanxiaobao.xyz/Article/details/guvnxoktd.sHtML

[R13] for 计数循环
来源：http://mobile.fanxiaobao.xyz/Article/details/gitxufcvj.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gymheikjr.sHtML

[R14] C 风格 for
来源：http://wap.fanxiaobao.xyz/Article/details/gzydpwjbs.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gxazmwlea.sHtML

[R15] while 逐行读文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gzbnjxlay.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gnxmtvuco.sHtML

[R16] until 等待条件
来源：http://3g.fanxiaobao.xyz/Article/details/ggedizvmd.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.fanxiaobao.xyz/Article/details/gqhknsoqn.sHtML

[R17] 数组定义与取值
来源：http://wap.fanxiaobao.xyz/Article/details/gwfetexhn.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.fanxiaobao.xyz/Article/details/gsgmfqnii.sHtML

[R18] 遍历数组
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmntblsvj.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.fanxiaobao.xyz/Article/details/gvudwmleo.sHtML

[R19] 数组长度
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyjdhhqli.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjiemntur.sHtML

[R20] 关联数组（字典）
来源：http://baike.fanxiaobao.xyz/Article/details/gwznlewvp.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wap.fanxiaobao.xyz/Article/details/gkfuvvccd.sHtML

[R21] 字符串长度
来源：http://www.share.fanxiaobao.xyz/Article/details/godqcapqi.sHtML

echo "${#s}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzjxqnbzf.sHtML

[R22] 截取子串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gghltyilr.sHtML

echo "${s:0:5}"
来源：http://3g.fanxiaobao.xyz/Article/details/gfhgjkfgw.sHtML

[R23] 字符串替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/giofishex.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.fanxiaobao.xyz/Article/details/gmfusxksy.sHtML

[R24] 大小写转换
来源：http://m.share.fanxiaobao.xyz/Article/details/gjomumnuc.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.fanxiaobao.xyz/Article/details/giupascrc.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.fanxiaobao.xyz/Article/details/gjoablwvk.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gvppoabbk.sHtML

[R26] 命令替换
来源：http://baike.fanxiaobao.xyz/Article/details/gdbnbwduf.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.fanxiaobao.xyz/Article/details/ghhcwcovm.sHtML

[R27] 算术展开
来源：http://wap.fanxiaobao.xyz/Article/details/gveegsrqq.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmawgprxa.sHtML

[R28] 浮点运算
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsvklschy.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.fanxiaobao.xyz/Article/details/gtstvqkdw.sHtML

[R29] 定义函数
来源：http://m.share.fanxiaobao.xyz/Article/details/goicqzcia.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.fanxiaobao.xyz/Article/details/ghhkgyrwt.sHtML

[R30] 函数返回状态码
来源：http://3g.fanxiaobao.xyz/Article/details/grhigkxpq.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.fanxiaobao.xyz/Article/details/gsqjihpgx.sHtML

[R31] 局部变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyloelqbl.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtgdbwhdt.sHtML

[R32] 参数个数校验
来源：http://3g.fanxiaobao.xyz/Article/details/geajzeulz.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.fanxiaobao.xyz/Article/details/ghkqbrzcd.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvgybgism.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.fanxiaobao.xyz/Article/details/glmxcwkcc.sHtML

[R34] 退出时清理
来源：http://baike.fanxiaobao.xyz/Article/details/gtvqpawzh.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.fanxiaobao.xyz/Article/details/goeflocfp.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmwqjxzqa.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.fanxiaobao.xyz/Article/details/gvsqizknh.sHtML

[R36] 并发执行多个任务
来源：http://www.share.fanxiaobao.xyz/Article/details/gtowijkxx.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghpvjebpo.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glkfxqrvj.sHtML

files=$(ls -1)
来源：http://mobile.fanxiaobao.xyz/Article/details/gdgguxpqr.sHtML

[R38] 管道串联
来源：http://3g.fanxiaobao.xyz/Article/details/glbthohav.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.fanxiaobao.xyz/Article/details/ggcudeyes.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.fanxiaobao.xyz/Article/details/glozgkwrn.sHtML

cmd > out.log 2>&1
来源：http://read.share.fanxiaobao.xyz/Article/details/ghrvazajx.sHtML

[R40] 追加写日志
来源：http://baike.fanxiaobao.xyz/Article/details/ggcmpikaw.sHtML

echo "log" >> out.log
来源：http://read.share.fanxiaobao.xyz/Article/details/gfzbkvywu.sHtML

[R41] 丢弃输出
来源：http://m.share.fanxiaobao.xyz/Article/details/gumlhfslv.sHtML

cmd >/dev/null 2>&1
来源：http://mobile.fanxiaobao.xyz/Article/details/ginefsaum.sHtML

[R42] 输入重定向
来源：http://blog.fanxiaobao.xyz/Article/details/gncyqhkjr.sHtML

wc -l < a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/glnpqzhsr.sHtML

[R43] 按名字查找文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gitrgsnxn.sHtML

find . -name "*.log" -type f
来源：http://blog.fanxiaobao.xyz/Article/details/gtnarnotq.sHtML

[R44] 按修改时间查找
来源：http://read.share.fanxiaobao.xyz/Article/details/glxqwfkia.sHtML

find . -mtime -7 -type f
来源：http://3g.fanxiaobao.xyz/Article/details/gzhlwtlzk.sHtML

[R45] 批量删除
来源：http://read.share.fanxiaobao.xyz/Article/details/gnjnugofz.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.fanxiaobao.xyz/Article/details/guqtienjn.sHtML

[R46] 递归替换文件内容
来源：http://3g.fanxiaobao.xyz/Article/details/gdxeyotfz.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.fanxiaobao.xyz/Article/details/gfvoqlqon.sHtML

[R47] sed 单行替换
来源：http://3g.fanxiaobao.xyz/Article/details/glxlhwpye.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gokppgdty.sHtML

[R48] awk 取指定列
来源：http://www.share.fanxiaobao.xyz/Article/details/gqxpglhsw.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gvdaxbpkh.sHtML

[R49] awk 带条件
来源：http://mobile.fanxiaobao.xyz/Article/details/gbkhkksnd.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.fanxiaobao.xyz/Article/details/giumzhlju.sHtML

[R50] awk 求和
来源：http://wap.fanxiaobao.xyz/Article/details/gnfisxcbm.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gzegblgrk.sHtML

[R51] 排序去重取前几
来源：http://baike.fanxiaobao.xyz/Article/details/ggkuhnwdp.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.fanxiaobao.xyz/Article/details/ggrdtxktf.sHtML

[R52] 统计行数
来源：http://wap.fanxiaobao.xyz/Article/details/gysoavqdu.sHtML

wc -l a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gasmbuqhj.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.fanxiaobao.xyz/Article/details/gapebxobz.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.fanxiaobao.xyz/Article/details/gtnnstxkf.sHtML

[R54] 比较两个文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gdsbsnjok.sHtML

diff a.txt b.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/guqhotznc.sHtML

[R55] 压缩与解压
来源：http://mobile.fanxiaobao.xyz/Article/details/gnmxmjyxf.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.fanxiaobao.xyz/Article/details/gswlkqqzo.sHtML

[R56] 远程拷贝
来源：http://baike.fanxiaobao.xyz/Article/details/ggpksjptp.sHtML

scp file user@host:/path/
来源：http://read.share.fanxiaobao.xyz/Article/details/gskyidtub.sHtML

[R57] 远程执行命令
来源：http://baike.fanxiaobao.xyz/Article/details/gfbkonzzb.sHtML

ssh user@host 'uptime'
来源：http://m.share.fanxiaobao.xyz/Article/details/gsrqjzaec.sHtML

[R58] 下载文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gvkejocjt.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.fanxiaobao.xyz/Article/details/gjptnsmhi.sHtML

[R59] 发 POST JSON
来源：http://wap.fanxiaobao.xyz/Article/details/gxarbrmbp.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.fanxiaobao.xyz/Article/details/gkavdggld.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.fanxiaobao.xyz/Article/details/gzlwbrvuc.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.fanxiaobao.xyz/Article/details/gpbpcnmxc.sHtML

[R61] 磁盘占用
来源：http://read.share.fanxiaobao.xyz/Article/details/gwrptnnoc.sHtML

df -h;  du -sh *
来源：http://mobile.fanxiaobao.xyz/Article/details/giluzszxx.sHtML

[R62] 找最占空间的文件
来源：http://blog.fanxiaobao.xyz/Article/details/gipjyplhf.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.fanxiaobao.xyz/Article/details/gkzsomsej.sHtML

[R63] 内存与进程
来源：http://3g.fanxiaobao.xyz/Article/details/gbkrkgeje.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.fanxiaobao.xyz/Article/details/grhipsztm.sHtML

[R64] 结束进程
来源：http://read.share.fanxiaobao.xyz/Article/details/ggadhgypt.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.fanxiaobao.xyz/Article/details/goeteohxl.sHtML

[R65] 查看端口占用
来源：http://3g.fanxiaobao.xyz/Article/details/gxnqgaebv.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.fanxiaobao.xyz/Article/details/gfmiyqygj.sHtML

[R66] 定时任务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwdtuuncd.sHtML

crontab -e;  crontab -l
来源：http://read.share.fanxiaobao.xyz/Article/details/gmnyemwjn.sHtML

[R67] 生成随机十六进制串
来源：http://baike.fanxiaobao.xyz/Article/details/gdbaubllg.sHtML

openssl rand -hex 16
来源：http://www.blog.fanxiaobao.xyz/Article/details/gitlmmakz.sHtML

[R68] 计算文件校验值
来源：http://read.share.fanxiaobao.xyz/Article/details/gttiricuk.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gnvquuhgb.sHtML

[R69] 生成随机密码
来源：http://3g.fanxiaobao.xyz/Article/details/gaxbhvipc.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.fanxiaobao.xyz/Article/details/ghmkuwldj.sHtML

[R70] 时间戳与互转
来源：http://read.share.fanxiaobao.xyz/Article/details/gnbxouqdp.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.fanxiaobao.xyz/Article/details/gsgrzqeyf.sHtML

[R71] 日期格式化
来源：http://www.share.fanxiaobao.xyz/Article/details/gymdmupmf.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.fanxiaobao.xyz/Article/details/gtnalgkls.sHtML

[R72] 等待端口就绪
来源：http://mobile.fanxiaobao.xyz/Article/details/gguvwsvcw.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gazcyiftv.sHtML

[R73] 分割大日志
来源：http://baike.fanxiaobao.xyz/Article/details/gbpovgiku.sHtML

split -l 1000 big.log part_
来源：http://blog.fanxiaobao.xyz/Article/details/ghqknfwot.sHtML

[R74] 批量重命名
来源：http://mobile.fanxiaobao.xyz/Article/details/gzlokjywv.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.fanxiaobao.xyz/Article/details/ggaptyxog.sHtML

[R75] 导出环境变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsryxzear.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.fanxiaobao.xyz/Article/details/gtzaeekfp.sHtML

[R76] 使用临时文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gvrsmhkcy.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.fanxiaobao.xyz/Article/details/gjivtaubr.sHtML

[R77] 读取用户输入
来源：http://baike.fanxiaobao.xyz/Article/details/gvovfasuv.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcqanukhp.sHtML

[R78] 交互式菜单
来源：http://blog.fanxiaobao.xyz/Article/details/ghnmpyfdv.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gknomkihx.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtswpoffo.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcytxmben.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.fanxiaobao.xyz/Article/details/ghawaqdng.sHtML

time ./run.sh
来源：http://blog.fanxiaobao.xyz/Article/details/gcmeoilhr.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gvjfbsyza.sHtML

S. C / C++ 专题
来源：http://m.share.fanxiaobao.xyz/Article/details/gxtwfrupn.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsdytsvnh.sHtML

[S01] C：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gykkxpsvz.sHtML

#include <stdio.h>
来源：http://www.share.fanxiaobao.xyz/Article/details/goqdtpela.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.fanxiaobao.xyz/Article/details/gbdhqzhho.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.fanxiaobao.xyz/Article/details/gflocwllp.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.fanxiaobao.xyz/Article/details/gxymbcmfu.sHtML

[S03] C：读入整数
来源：http://read.share.fanxiaobao.xyz/Article/details/gbxdqztot.sHtML

int x; scanf("%d", &x);
来源：http://read.share.fanxiaobao.xyz/Article/details/gbojejfih.sHtML

[S04] C：字符串复制
来源：http://wap.fanxiaobao.xyz/Article/details/gfyefduac.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzjdwxjsv.sHtML

[S05] C：字符串长度
来源：http://baike.fanxiaobao.xyz/Article/details/gxgbgkwyb.sHtML

strlen(s)
来源：http://read.share.fanxiaobao.xyz/Article/details/gungdpumh.sHtML

[S06] C：字符串比较
来源：http://baike.fanxiaobao.xyz/Article/details/gzkdpmpyg.sHtML

strcmp(a, b) == 0
来源：http://blog.fanxiaobao.xyz/Article/details/gydylfmgf.sHtML

[S07] C：数组遍历求和
来源：http://baike.fanxiaobao.xyz/Article/details/gjepxcvbs.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.fanxiaobao.xyz/Article/details/grahkrdje.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.fanxiaobao.xyz/Article/details/gzcbodtyc.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.fanxiaobao.xyz/Article/details/gxrshnrkb.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.fanxiaobao.xyz/Article/details/gwwlensxv.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.fanxiaobao.xyz/Article/details/gutdqjftc.sHtML

[S10] C：指针与解引用
来源：http://baike.fanxiaobao.xyz/Article/details/grlmkmlhl.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkzrzlyns.sHtML

[S11] C：逐行读文件
来源：http://wap.fanxiaobao.xyz/Article/details/goldfczlf.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwofnasrd.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.fanxiaobao.xyz/Article/details/guyvnpwcp.sHtML

fclose(f);
来源：http://www.share.fanxiaobao.xyz/Article/details/gymlbutyd.sHtML

[S12] C：写文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gicamtwkq.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.fanxiaobao.xyz/Article/details/gmntniowe.sHtML

[S13] C：宏定义
来源：http://www.share.fanxiaobao.xyz/Article/details/gdafjmnuo.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.fanxiaobao.xyz/Article/details/gsowqtopn.sHtML

[S14] C：枚举
来源：http://blog.fanxiaobao.xyz/Article/details/gjwxfxoas.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.fanxiaobao.xyz/Article/details/gnvzpjama.sHtML

[S15] C：类型转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggfrjizka.sHtML

(double) a / b
来源：http://wap.fanxiaobao.xyz/Article/details/gewhoakob.sHtML

[S16] C：位操作置位
来源：http://3g.fanxiaobao.xyz/Article/details/gsyfcxgxz.sHtML

x |= (1 << 3);
来源：http://read.share.fanxiaobao.xyz/Article/details/gdfzyrggg.sHtML

[S17] C：安全拼接字符串
来源：http://wap.fanxiaobao.xyz/Article/details/giqcjfevq.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grlzzgsss.sHtML

[S18] C：命令行参数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gowukhcpt.sHtML

int main(int argc, char **argv)
来源：http://m.share.fanxiaobao.xyz/Article/details/gjcczwyoo.sHtML

[S19] C：快速排序
来源：http://read.share.fanxiaobao.xyz/Article/details/gmbaplcsp.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.fanxiaobao.xyz/Article/details/gtktbwvag.sHtML

[S20] C：二分查找
来源：http://baike.fanxiaobao.xyz/Article/details/gnbdqtpry.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.fanxiaobao.xyz/Article/details/gcdkpyzei.sHtML

[S21] C：字符类别判断
来源：http://blog.fanxiaobao.xyz/Article/details/gxtkezdnz.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.fanxiaobao.xyz/Article/details/gsjmzhews.sHtML

[S22] C：字符串转数字
来源：http://read.share.fanxiaobao.xyz/Article/details/geanyabhn.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.fanxiaobao.xyz/Article/details/gslrksnaz.sHtML

[S23] C：随机数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwezwaskc.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.fanxiaobao.xyz/Article/details/gfnbgzcft.sHtML

[S24] C：获取本地时间
来源：http://mobile.fanxiaobao.xyz/Article/details/gpsqgwfyi.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.fanxiaobao.xyz/Article/details/gazftxxsn.sHtML

[S25] C：内存拷贝
来源：http://www.share.fanxiaobao.xyz/Article/details/gzxtfbtyp.sHtML

memcpy(dst, src, n);
来源：http://blog.fanxiaobao.xyz/Article/details/gfgemfzta.sHtML

[S26] C：内存清零
来源：http://read.share.fanxiaobao.xyz/Article/details/gtfyqqwmj.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.fanxiaobao.xyz/Article/details/gbxneninr.sHtML

[S27] C：定义常量
来源：http://www.share.fanxiaobao.xyz/Article/details/gxtostaev.sHtML

const double PI = 3.14159;
来源：http://blog.fanxiaobao.xyz/Article/details/gybpoqywn.sHtML

[S28] C：静态变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gktvdveeo.sHtML

static int counter = 0;
来源：http://wap.fanxiaobao.xyz/Article/details/ghmzxolai.sHtML

[S29] C：变参函数
来源：http://wap.fanxiaobao.xyz/Article/details/gsompcnvq.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.fanxiaobao.xyz/Article/details/giwidhlov.sHtML

[S30] C：头文件保护
来源：http://m.share.fanxiaobao.xyz/Article/details/gxoetghbr.sHtML

#ifndef X_H
来源：http://read.share.fanxiaobao.xyz/Article/details/gfzinnrpo.sHtML

#define X_H
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ganbgisnl.sHtML

#endif
来源：http://www.blog.fanxiaobao.xyz/Article/details/gddkkcuuv.sHtML

[S31] C++：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gpbwjdvmy.sHtML

#include <iostream>
来源：http://read.share.fanxiaobao.xyz/Article/details/gutmgqdrz.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.fanxiaobao.xyz/Article/details/guoovjpwl.sHtML

[S32] C++：字符串
来源：http://blog.fanxiaobao.xyz/Article/details/gcoqxpmyq.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.fanxiaobao.xyz/Article/details/ggxpovejl.sHtML

[S33] C++：vector 增删
来源：http://blog.fanxiaobao.xyz/Article/details/gmfethrlt.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gegcvglms.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwqzmphep.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.fanxiaobao.xyz/Article/details/gekffzdum.sHtML

[S35] C++：map
来源：http://baike.fanxiaobao.xyz/Article/details/gvtkfggjy.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/ghlnjnvsb.sHtML

[S36] C++：unordered_map
来源：http://3g.fanxiaobao.xyz/Article/details/gzshulmge.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gyrlyeoxn.sHtML

[S37] C++：set
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gftbmhmfl.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.fanxiaobao.xyz/Article/details/gmarsykod.sHtML

[S38] C++：排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbihuuuav.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.fanxiaobao.xyz/Article/details/gwrfzqchh.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.fanxiaobao.xyz/Article/details/gjgvkdtkx.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxnrqodmk.sHtML

[S40] C++：查找元素
来源：http://mobile.fanxiaobao.xyz/Article/details/gmlxybbcs.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.fanxiaobao.xyz/Article/details/gpocwslqg.sHtML

[S41] C++：类与构造函数
来源：http://wap.fanxiaobao.xyz/Article/details/geaulrdkf.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.fanxiaobao.xyz/Article/details/gagksjoox.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjwajgkit.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.fanxiaobao.xyz/Article/details/gmlpxmwrb.sHtML

[S43] C++：智能指针
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gttwcjrxz.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.fanxiaobao.xyz/Article/details/goajnybok.sHtML

[S44] C++：引用传参
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnithejpj.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gggxcqtzh.sHtML

[S45] C++：lambda
来源：http://baike.fanxiaobao.xyz/Article/details/gvwobevla.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggtczmatu.sHtML

[S46] C++：函数模板
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmljsyebp.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.fanxiaobao.xyz/Article/details/gtienrelo.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.fanxiaobao.xyz/Article/details/gvqonokkl.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.fanxiaobao.xyz/Article/details/gzuciyjyu.sHtML

[S48] C++：逐行读文件
来源：http://baike.fanxiaobao.xyz/Article/details/guqcwvtus.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.fanxiaobao.xyz/Article/details/gkyaeqnaw.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gticygljj.sHtML

[S49] C++：写文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxgnzyaip.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.fanxiaobao.xyz/Article/details/gihzblvol.sHtML

[S50] C++：格式化数字
来源：http://blog.fanxiaobao.xyz/Article/details/gdlqifpyv.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.fanxiaobao.xyz/Article/details/gvewjpyos.sHtML

[S51] C++：显式类型转换
来源：http://wap.fanxiaobao.xyz/Article/details/gbliylbwo.sHtML

static_cast<double>(a) / b
来源：http://m.share.fanxiaobao.xyz/Article/details/gegcdrwva.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxztjiyxh.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gsvotqzms.sHtML

[S53] C++：移动语义
来源：http://mobile.fanxiaobao.xyz/Article/details/glijgwzym.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.fanxiaobao.xyz/Article/details/gqlwbcisl.sHtML

[S54] C++：异常处理
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtxtdyqft.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.fanxiaobao.xyz/Article/details/gszlykdpk.sHtML

[S55] C++：结构化绑定
来源：http://3g.fanxiaobao.xyz/Article/details/gxxiprrrp.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.fanxiaobao.xyz/Article/details/gmohmlubx.sHtML

[S56] C++：optional
来源：http://www.blog.fanxiaobao.xyz/Article/details/govyobkvp.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.fanxiaobao.xyz/Article/details/gbrpiirbt.sHtML

[S57] C++：编译期常量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gllvwywmo.sHtML

constexpr int N = 10;
来源：http://m.share.fanxiaobao.xyz/Article/details/gykrjzgby.sHtML

[S58] C++：命名空间
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvvzbxtno.sHtML

namespace ns { int f() { return 1; } }
来源：http://blog.fanxiaobao.xyz/Article/details/gwyjonwuf.sHtML

[S59] C++：静态断言
来源：http://wap.fanxiaobao.xyz/Article/details/gaaocoouk.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.fanxiaobao.xyz/Article/details/gepxbxhpr.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.fanxiaobao.xyz/Article/details/gugspjbcw.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.fanxiaobao.xyz/Article/details/gndmjbykw.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/ghfgxqqsh.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.fanxiaobao.xyz/Article/details/gykhczmsk.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gmupvpizo.sHtML

[T01] Kotlin：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gceaepkbx.sHtML

println("Hello")
来源：http://www.share.fanxiaobao.xyz/Article/details/gtzlcqxcg.sHtML

[T02] Kotlin：变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gscnpmjuz.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.fanxiaobao.xyz/Article/details/gjnddngea.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.fanxiaobao.xyz/Article/details/gerxbdhfs.sHtML

"值: $b"
来源：http://blog.fanxiaobao.xyz/Article/details/glmcmmoih.sHtML

[T04] Kotlin：空安全
来源：http://m.share.fanxiaobao.xyz/Article/details/gfzistdfr.sHtML

val n: String? = null;  n?.length
来源：http://read.share.fanxiaobao.xyz/Article/details/gmjlptjnk.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.fanxiaobao.xyz/Article/details/gytrcawlh.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.fanxiaobao.xyz/Article/details/gibntffox.sHtML

[T06] Kotlin：集合映射
来源：http://baike.fanxiaobao.xyz/Article/details/giiwdqjbl.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.fanxiaobao.xyz/Article/details/gfmyjntud.sHtML

[T07] Kotlin：集合过滤
来源：http://blog.fanxiaobao.xyz/Article/details/gudkzolpt.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.fanxiaobao.xyz/Article/details/ginzivpxf.sHtML

[T08] Kotlin：数据类
来源：http://m.share.fanxiaobao.xyz/Article/details/gdnrpzngr.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.fanxiaobao.xyz/Article/details/gnzenakcg.sHtML


<!-- 参考信息 -->