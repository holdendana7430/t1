代发 wailian999

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.fanxiaobao.xyz/Article/details/ggrgkbwoo.sHtML

[R08] 数值比较
来源：http://3g.fanxiaobao.xyz/Article/details/gwzsyzxqt.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://m.share.fanxiaobao.xyz/Article/details/gnihepqkv.sHtML

[R09] 字符串比较
来源：http://www.share.fanxiaobao.xyz/Article/details/gnfgwygxe.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/gikyxjvyp.sHtML

[R10] 正则匹配
来源：http://wap.fanxiaobao.xyz/Article/details/gzjskyigd.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.fanxiaobao.xyz/Article/details/gujpimmhx.sHtML

[R11] case 多分支
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gihhkhnro.sHtML

case "$1" in
来源：http://mobile.fanxiaobao.xyz/Article/details/gzqjnukzz.sHtML

start) echo "启动" ;;
来源：http://blog.fanxiaobao.xyz/Article/details/goookmkgx.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfkpysxwa.sHtML

*)     echo "未知命令" ;;
来源：http://baike.fanxiaobao.xyz/Article/details/glgkoxlvi.sHtML

esac
来源：http://read.share.fanxiaobao.xyz/Article/details/gbxxblmew.sHtML

[R12] for 遍历文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gwjsgvupb.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/giqcmjkkx.sHtML

[R13] for 计数循环
来源：http://baike.fanxiaobao.xyz/Article/details/gjlvxuzxi.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gebdbjmnh.sHtML

[R14] C 风格 for
来源：http://blog.fanxiaobao.xyz/Article/details/grbxsczkp.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://baike.fanxiaobao.xyz/Article/details/gxusjriom.sHtML

[R15] while 逐行读文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gsjprrjkv.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/glrtvmlfn.sHtML

[R16] until 等待条件
来源：http://3g.fanxiaobao.xyz/Article/details/gfopvjifa.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqdriodrm.sHtML

[R17] 数组定义与取值
来源：http://read.share.fanxiaobao.xyz/Article/details/gncaxniux.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gajziaidg.sHtML

[R18] 遍历数组
来源：http://read.share.fanxiaobao.xyz/Article/details/grhrssjvr.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.fanxiaobao.xyz/Article/details/gujatmfoq.sHtML

[R19] 数组长度
来源：http://read.share.fanxiaobao.xyz/Article/details/gsaaykklk.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwqmwalqz.sHtML

[R20] 关联数组（字典）
来源：http://m.share.fanxiaobao.xyz/Article/details/gkvnwpcho.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.fanxiaobao.xyz/Article/details/gtdtuhtim.sHtML

[R21] 字符串长度
来源：http://blog.fanxiaobao.xyz/Article/details/gidngqbgr.sHtML

echo "${#s}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmbbnasui.sHtML

[R22] 截取子串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwwqzzyki.sHtML

echo "${s:0:5}"
来源：http://baike.fanxiaobao.xyz/Article/details/gqbjkyrvz.sHtML

[R23] 字符串替换
来源：http://3g.fanxiaobao.xyz/Article/details/gwymstddc.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gekvhlxzn.sHtML

[R24] 大小写转换
来源：http://blog.fanxiaobao.xyz/Article/details/gsaynghxs.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gsvqcosuq.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.fanxiaobao.xyz/Article/details/gsdritagd.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqkjpsusr.sHtML

[R26] 命令替换
来源：http://read.share.fanxiaobao.xyz/Article/details/ghziaqwxg.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbtrrizdh.sHtML

[R27] 算术展开
来源：http://baike.fanxiaobao.xyz/Article/details/gopuliejj.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.fanxiaobao.xyz/Article/details/gfbhbpumi.sHtML

[R28] 浮点运算
来源：http://wap.fanxiaobao.xyz/Article/details/goncytzvw.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.fanxiaobao.xyz/Article/details/gulhorluh.sHtML

[R29] 定义函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gscbbttlp.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.fanxiaobao.xyz/Article/details/gvqhugiss.sHtML

[R30] 函数返回状态码
来源：http://www.share.fanxiaobao.xyz/Article/details/gzvlpuwgc.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.fanxiaobao.xyz/Article/details/gqyxrhriz.sHtML

[R31] 局部变量
来源：http://3g.fanxiaobao.xyz/Article/details/gcrypsiph.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grvwkmgxv.sHtML

[R32] 参数个数校验
来源：http://3g.fanxiaobao.xyz/Article/details/ggmfdjzdq.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.fanxiaobao.xyz/Article/details/gzqyveapq.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.fanxiaobao.xyz/Article/details/gbbcmlwdr.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpfctahqs.sHtML

[R34] 退出时清理
来源：http://m.share.fanxiaobao.xyz/Article/details/gxktxsvem.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fanxiaobao.xyz/Article/details/gfsrfscwq.sHtML

[R35] 后台执行并等待
来源：http://baike.fanxiaobao.xyz/Article/details/girwafgme.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.fanxiaobao.xyz/Article/details/gildrsrpo.sHtML

[R36] 并发执行多个任务
来源：http://www.share.fanxiaobao.xyz/Article/details/gkbqaogxp.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.fanxiaobao.xyz/Article/details/gwljaedua.sHtML

[R37] 把输出赋给变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gnlpmcgad.sHtML

files=$(ls -1)
来源：http://baike.fanxiaobao.xyz/Article/details/gsvizbfnz.sHtML

[R38] 管道串联
来源：http://baike.fanxiaobao.xyz/Article/details/giveafepa.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.fanxiaobao.xyz/Article/details/ggvpdufzg.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.fanxiaobao.xyz/Article/details/ggbadyzzd.sHtML

cmd > out.log 2>&1
来源：http://www.share.fanxiaobao.xyz/Article/details/glfpitpbu.sHtML

[R40] 追加写日志
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbbpghhmr.sHtML

echo "log" >> out.log
来源：http://baike.fanxiaobao.xyz/Article/details/gzuhqgont.sHtML

[R41] 丢弃输出
来源：http://www.share.fanxiaobao.xyz/Article/details/gnmaktikq.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guuqypbch.sHtML

[R42] 输入重定向
来源：http://3g.fanxiaobao.xyz/Article/details/gsfghusbm.sHtML

wc -l < a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gsanalbcl.sHtML

[R43] 按名字查找文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gglkxtskp.sHtML

find . -name "*.log" -type f
来源：http://www.share.fanxiaobao.xyz/Article/details/gbgansorf.sHtML

[R44] 按修改时间查找
来源：http://mobile.fanxiaobao.xyz/Article/details/gbnptnrca.sHtML

find . -mtime -7 -type f
来源：http://baike.fanxiaobao.xyz/Article/details/gtgqibppo.sHtML

[R45] 批量删除
来源：http://read.share.fanxiaobao.xyz/Article/details/gmfpfgwss.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.fanxiaobao.xyz/Article/details/ggkothjbu.sHtML

[R46] 递归替换文件内容
来源：http://mobile.fanxiaobao.xyz/Article/details/gfxjpkdtt.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.fanxiaobao.xyz/Article/details/gwjopjdyz.sHtML

[R47] sed 单行替换
来源：http://blog.fanxiaobao.xyz/Article/details/gowxkzoqi.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gbowpotqc.sHtML

[R48] awk 取指定列
来源：http://3g.fanxiaobao.xyz/Article/details/gzcfgekvs.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/ggwlrfxsx.sHtML

[R49] awk 带条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggvucpdjo.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmngmxmxz.sHtML

[R50] awk 求和
来源：http://read.share.fanxiaobao.xyz/Article/details/gvqylwhnl.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gowhntkci.sHtML

[R51] 排序去重取前几
来源：http://m.share.fanxiaobao.xyz/Article/details/gjpmwxtmh.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.fanxiaobao.xyz/Article/details/gwordwfha.sHtML

[R52] 统计行数
来源：http://blog.fanxiaobao.xyz/Article/details/gvtkpuapz.sHtML

wc -l a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giwwgfwoc.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.fanxiaobao.xyz/Article/details/gpqnlfonu.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.fanxiaobao.xyz/Article/details/gkzrrcudg.sHtML

[R54] 比较两个文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmhbvetga.sHtML

diff a.txt b.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/glivtgncn.sHtML

[R55] 压缩与解压
来源：http://m.share.fanxiaobao.xyz/Article/details/gdhxfddaw.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.fanxiaobao.xyz/Article/details/gphlqsnce.sHtML

[R56] 远程拷贝
来源：http://3g.fanxiaobao.xyz/Article/details/gihrqfvpp.sHtML

scp file user@host:/path/
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsovygxbl.sHtML

[R57] 远程执行命令
来源：http://blog.fanxiaobao.xyz/Article/details/gjzlscnpt.sHtML

ssh user@host 'uptime'
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjjplqlna.sHtML

[R58] 下载文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gvlpqjxnn.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzwjoeyrn.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfgimnzlk.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.fanxiaobao.xyz/Article/details/gqbcttyka.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdspwzivi.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.fanxiaobao.xyz/Article/details/gziecnwuc.sHtML

[R61] 磁盘占用
来源：http://blog.fanxiaobao.xyz/Article/details/gbgnmqpai.sHtML

df -h;  du -sh *
来源：http://baike.fanxiaobao.xyz/Article/details/gvqekabzm.sHtML

[R62] 找最占空间的文件
来源：http://wap.fanxiaobao.xyz/Article/details/gsptgeiqg.sHtML

du -ah . | sort -rh | head -10
来源：http://3g.fanxiaobao.xyz/Article/details/ghtkaquen.sHtML

[R63] 内存与进程
来源：http://read.share.fanxiaobao.xyz/Article/details/ghnqrprwm.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjftpmmls.sHtML

[R64] 结束进程
来源：http://blog.fanxiaobao.xyz/Article/details/gpoizgwjj.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.fanxiaobao.xyz/Article/details/gnxfgtmby.sHtML

[R65] 查看端口占用
来源：http://m.share.fanxiaobao.xyz/Article/details/gzdnpedsk.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.fanxiaobao.xyz/Article/details/gemwfozog.sHtML

[R66] 定时任务
来源：http://baike.fanxiaobao.xyz/Article/details/gplzbkeaz.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggqeghmlq.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.fanxiaobao.xyz/Article/details/gqvpwcodb.sHtML

openssl rand -hex 16
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glhwflefq.sHtML

[R68] 计算文件校验值
来源：http://mobile.fanxiaobao.xyz/Article/details/gzcktbbie.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gstgsumtc.sHtML

[R69] 生成随机密码
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxlqqgdtr.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.fanxiaobao.xyz/Article/details/gcbzqdgha.sHtML

[R70] 时间戳与互转
来源：http://read.share.fanxiaobao.xyz/Article/details/gsscwqixi.sHtML

date +%s;  date -d @1700000000
来源：http://3g.fanxiaobao.xyz/Article/details/gefszeftk.sHtML

[R71] 日期格式化
来源：http://m.share.fanxiaobao.xyz/Article/details/ghjvebzdu.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.fanxiaobao.xyz/Article/details/guhicyydw.sHtML

[R72] 等待端口就绪
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbjosnstv.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.fanxiaobao.xyz/Article/details/gypyjisxl.sHtML

[R73] 分割大日志
来源：http://wap.fanxiaobao.xyz/Article/details/gwmuzaoce.sHtML

split -l 1000 big.log part_
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaofwklxo.sHtML

[R74] 批量重命名
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvwubejan.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gosmjlvpz.sHtML

[R75] 导出环境变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gnypslxlp.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.fanxiaobao.xyz/Article/details/gtpgzcewn.sHtML

[R76] 使用临时文件
来源：http://mobile.fanxiaobao.xyz/Article/details/ghrdgykyi.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqhwtfakh.sHtML

[R77] 读取用户输入
来源：http://read.share.fanxiaobao.xyz/Article/details/glybwndbz.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxwrejkyx.sHtML

[R78] 交互式菜单
来源：http://read.share.fanxiaobao.xyz/Article/details/gcygqgrlh.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gvlvmawkr.sHtML

[R79] 解析命令行选项
来源：http://mobile.fanxiaobao.xyz/Article/details/ghrxjjkuw.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.fanxiaobao.xyz/Article/details/gquejstyw.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glfbjhlxe.sHtML

time ./run.sh
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvuesrdtq.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/glpstejjs.sHtML

S. C / C++ 专题
来源：http://www.blog.fanxiaobao.xyz/Article/details/guzsxyuwj.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gmkaprtpd.sHtML

[S01] C：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gjnwuozsw.sHtML

#include <stdio.h>
来源：http://read.share.fanxiaobao.xyz/Article/details/guyjzvlrx.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.fanxiaobao.xyz/Article/details/ghnwbyzri.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfbwlsshy.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.fanxiaobao.xyz/Article/details/gasixjhyb.sHtML

[S03] C：读入整数
来源：http://3g.fanxiaobao.xyz/Article/details/gjfwaqbgb.sHtML

int x; scanf("%d", &x);
来源：http://baike.fanxiaobao.xyz/Article/details/gzmsxoqbl.sHtML

[S04] C：字符串复制
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqpivuksa.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.fanxiaobao.xyz/Article/details/gkfpcizay.sHtML

[S05] C：字符串长度
来源：http://read.share.fanxiaobao.xyz/Article/details/gkwnbncui.sHtML

strlen(s)
来源：http://read.share.fanxiaobao.xyz/Article/details/ghbuzwyfe.sHtML

[S06] C：字符串比较
来源：http://read.share.fanxiaobao.xyz/Article/details/grkkgjwch.sHtML

strcmp(a, b) == 0
来源：http://read.share.fanxiaobao.xyz/Article/details/gjdgebnym.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gatinnvsh.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.fanxiaobao.xyz/Article/details/gjrtwezty.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.fanxiaobao.xyz/Article/details/gnsfwnpbf.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.fanxiaobao.xyz/Article/details/gmjkutifh.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdizatmyh.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.fanxiaobao.xyz/Article/details/ghlmgjsky.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsavemogx.sHtML

int *p = &a;  *p = 5;
来源：http://wap.fanxiaobao.xyz/Article/details/gbyzrnwrn.sHtML

[S11] C：逐行读文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gaqncnuni.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.fanxiaobao.xyz/Article/details/ghjdelwuz.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.fanxiaobao.xyz/Article/details/gticmafag.sHtML

fclose(f);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdrqphbps.sHtML

[S12] C：写文件
来源：http://3g.fanxiaobao.xyz/Article/details/guqgwyrxw.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.fanxiaobao.xyz/Article/details/gtwxmshbr.sHtML

[S13] C：宏定义
来源：http://mobile.fanxiaobao.xyz/Article/details/guwyijprq.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.fanxiaobao.xyz/Article/details/gcmrdecdo.sHtML

[S14] C：枚举
来源：http://read.share.fanxiaobao.xyz/Article/details/ghfzuygsu.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.fanxiaobao.xyz/Article/details/gdzxvlpcs.sHtML

[S15] C：类型转换
来源：http://blog.fanxiaobao.xyz/Article/details/gpvvbxcay.sHtML

(double) a / b
来源：http://3g.fanxiaobao.xyz/Article/details/gwtdnfocc.sHtML

[S16] C：位操作置位
来源：http://mobile.fanxiaobao.xyz/Article/details/gnjplsbdx.sHtML

x |= (1 << 3);
来源：http://www.share.fanxiaobao.xyz/Article/details/gdixawwmk.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.fanxiaobao.xyz/Article/details/guldruwdz.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.fanxiaobao.xyz/Article/details/glpkdlowf.sHtML

[S18] C：命令行参数
来源：http://m.share.fanxiaobao.xyz/Article/details/gatufiduz.sHtML

int main(int argc, char **argv)
来源：http://www.share.fanxiaobao.xyz/Article/details/gkzdfddlf.sHtML

[S19] C：快速排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/gozcvqtpl.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.fanxiaobao.xyz/Article/details/ggcsgggqj.sHtML

[S20] C：二分查找
来源：http://m.share.fanxiaobao.xyz/Article/details/gsvjypsdm.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.fanxiaobao.xyz/Article/details/gwfvfyrod.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwdbuuvdu.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.fanxiaobao.xyz/Article/details/genqkurky.sHtML

[S22] C：字符串转数字
来源：http://m.share.fanxiaobao.xyz/Article/details/gwxusqusc.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.fanxiaobao.xyz/Article/details/gjvrbmips.sHtML

[S23] C：随机数
来源：http://www.share.fanxiaobao.xyz/Article/details/gqbjgyhqt.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.fanxiaobao.xyz/Article/details/ggopmmhqu.sHtML

[S24] C：获取本地时间
来源：http://blog.fanxiaobao.xyz/Article/details/gznppijio.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.fanxiaobao.xyz/Article/details/gjjjylthz.sHtML

[S25] C：内存拷贝
来源：http://3g.fanxiaobao.xyz/Article/details/grlfhdmdk.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjmajnpye.sHtML

[S26] C：内存清零
来源：http://3g.fanxiaobao.xyz/Article/details/ghixiwlkv.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.fanxiaobao.xyz/Article/details/gepovlvrc.sHtML

[S27] C：定义常量
来源：http://mobile.fanxiaobao.xyz/Article/details/gmwymtadq.sHtML

const double PI = 3.14159;
来源：http://read.share.fanxiaobao.xyz/Article/details/gnfqxrcdm.sHtML

[S28] C：静态变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gtomhzwta.sHtML

static int counter = 0;
来源：http://mobile.fanxiaobao.xyz/Article/details/gznhjogff.sHtML

[S29] C：变参函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gpjrlecel.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.fanxiaobao.xyz/Article/details/gqxfxlnyu.sHtML

[S30] C：头文件保护
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvorluptb.sHtML

#ifndef X_H
来源：http://wap.fanxiaobao.xyz/Article/details/gizupmiuk.sHtML

#define X_H
来源：http://read.share.fanxiaobao.xyz/Article/details/ganerorrd.sHtML

#endif
来源：http://read.share.fanxiaobao.xyz/Article/details/grmjippvv.sHtML

[S31] C++：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gohfjhbad.sHtML

#include <iostream>
来源：http://3g.fanxiaobao.xyz/Article/details/grkygxzbl.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.fanxiaobao.xyz/Article/details/gkhfboerx.sHtML

[S32] C++：字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/gdalbhbhs.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxqfjtxdv.sHtML

[S33] C++：vector 增删
来源：http://3g.fanxiaobao.xyz/Article/details/gywisyaon.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.fanxiaobao.xyz/Article/details/gccqyfymn.sHtML

[S34] C++：遍历 vector
来源：http://m.share.fanxiaobao.xyz/Article/details/gzxjzhctz.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtkrryopd.sHtML

[S35] C++：map
来源：http://blog.fanxiaobao.xyz/Article/details/glwwzvfuf.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.fanxiaobao.xyz/Article/details/guuxvjtfl.sHtML

[S36] C++：unordered_map
来源：http://mobile.fanxiaobao.xyz/Article/details/gddjvqwtz.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/ghxtameff.sHtML

[S37] C++：set
来源：http://www.share.fanxiaobao.xyz/Article/details/gztpvmlza.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.fanxiaobao.xyz/Article/details/gunmqsxnj.sHtML

[S38] C++：排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwrwfgywn.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.fanxiaobao.xyz/Article/details/ggpuurxov.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.fanxiaobao.xyz/Article/details/ggwwxafwx.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.fanxiaobao.xyz/Article/details/gttjkogrc.sHtML

[S40] C++：查找元素
来源：http://www.share.fanxiaobao.xyz/Article/details/gqiuizkba.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.fanxiaobao.xyz/Article/details/gvcukixvc.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/ganzeqvgk.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.fanxiaobao.xyz/Article/details/gugfjnyki.sHtML

[S42] C++：继承与虚函数
来源：http://baike.fanxiaobao.xyz/Article/details/gouhwkcvu.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gccyaxhtd.sHtML

[S43] C++：智能指针
来源：http://3g.fanxiaobao.xyz/Article/details/gilyjzxfk.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.fanxiaobao.xyz/Article/details/gmbdbwfnt.sHtML

[S44] C++：引用传参
来源：http://baike.fanxiaobao.xyz/Article/details/gbdybvlhc.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gmjoqldnk.sHtML

[S45] C++：lambda
来源：http://baike.fanxiaobao.xyz/Article/details/gtwxpbait.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.fanxiaobao.xyz/Article/details/gqazxlcfc.sHtML

[S46] C++：函数模板
来源：http://m.share.fanxiaobao.xyz/Article/details/glotijste.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gquyrnwio.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.fanxiaobao.xyz/Article/details/gmugeakmq.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.fanxiaobao.xyz/Article/details/ghbugzxty.sHtML

[S48] C++：逐行读文件
来源：http://3g.fanxiaobao.xyz/Article/details/gwsnkrhtb.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://m.share.fanxiaobao.xyz/Article/details/gnwidroab.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gupwprdat.sHtML

[S49] C++：写文件
来源：http://baike.fanxiaobao.xyz/Article/details/gapudqrqc.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gknulgfzq.sHtML

[S50] C++：格式化数字
来源：http://3g.fanxiaobao.xyz/Article/details/gmwosyewa.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdjscztrr.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnuntpnxb.sHtML

static_cast<double>(a) / b
来源：http://blog.fanxiaobao.xyz/Article/details/gpjxhgozk.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.fanxiaobao.xyz/Article/details/geklnskkp.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gvxpcoxaa.sHtML

[S53] C++：移动语义
来源：http://3g.fanxiaobao.xyz/Article/details/gdrejurum.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.fanxiaobao.xyz/Article/details/gtpplplje.sHtML

[S54] C++：异常处理
来源：http://www.share.fanxiaobao.xyz/Article/details/ghyjxvlpa.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.fanxiaobao.xyz/Article/details/grlfrdvqn.sHtML

[S55] C++：结构化绑定
来源：http://blog.fanxiaobao.xyz/Article/details/gzfhvjbmv.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.fanxiaobao.xyz/Article/details/gccgaivws.sHtML

[S56] C++：optional
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmfhmdbhk.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.fanxiaobao.xyz/Article/details/grollyhpi.sHtML

[S57] C++：编译期常量
来源：http://mobile.fanxiaobao.xyz/Article/details/gysbmhghm.sHtML

constexpr int N = 10;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbpvgtnls.sHtML

[S58] C++：命名空间
来源：http://read.share.fanxiaobao.xyz/Article/details/gmltzbrqt.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.fanxiaobao.xyz/Article/details/gnkxpscqd.sHtML

[S59] C++：静态断言
来源：http://m.share.fanxiaobao.xyz/Article/details/gjzhwqfjr.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.fanxiaobao.xyz/Article/details/godyrsqfn.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.fanxiaobao.xyz/Article/details/gxycxawoj.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.fanxiaobao.xyz/Article/details/gqwswqctt.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gqufituyx.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.fanxiaobao.xyz/Article/details/gmuccfkkf.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gfxxctyau.sHtML

[T01] Kotlin：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/ggljxpbuo.sHtML

println("Hello")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvdgognzd.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggilwnyyc.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.fanxiaobao.xyz/Article/details/gemqfkgnp.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.fanxiaobao.xyz/Article/details/gngjqburb.sHtML

"值: $b"
来源：http://www.share.fanxiaobao.xyz/Article/details/gcpkngufm.sHtML

[T04] Kotlin：空安全
来源：http://baike.fanxiaobao.xyz/Article/details/grlrjggra.sHtML

val n: String? = null;  n?.length
来源：http://m.share.fanxiaobao.xyz/Article/details/giahaxuhg.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.fanxiaobao.xyz/Article/details/glqxdmige.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.fanxiaobao.xyz/Article/details/gzpxukcuf.sHtML

[T06] Kotlin：集合映射
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnawyruqo.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.fanxiaobao.xyz/Article/details/gtrsiswoe.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.fanxiaobao.xyz/Article/details/gxfytzxza.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.fanxiaobao.xyz/Article/details/gbiaubgvn.sHtML

[T08] Kotlin：数据类
来源：http://mobile.fanxiaobao.xyz/Article/details/gbwtgsdya.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.fanxiaobao.xyz/Article/details/gszwdpgxc.sHtML


<!-- 参考信息 -->