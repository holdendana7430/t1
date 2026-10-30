代发 wailian999

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://baike.fanxiaobao.xyz/Article/details/gyskbjqcw.sHtML

[R08] 数值比较
来源：http://www.share.fanxiaobao.xyz/Article/details/gcjadlyng.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/gtwzfvztm.sHtML

[R09] 字符串比较
来源：http://wap.fanxiaobao.xyz/Article/details/gfgcanjaf.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.fanxiaobao.xyz/Article/details/gkkpcfwgd.sHtML

[R10] 正则匹配
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gddrbxvtf.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.fanxiaobao.xyz/Article/details/geagexeec.sHtML

[R11] case 多分支
来源：http://m.share.fanxiaobao.xyz/Article/details/gwuhgedpu.sHtML

case "$1" in
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmvwdxgzl.sHtML

start) echo "启动" ;;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjsystewb.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glllbczcz.sHtML

*)     echo "未知命令" ;;
来源：http://wap.fanxiaobao.xyz/Article/details/gidwmchqw.sHtML

esac
来源：http://mobile.fanxiaobao.xyz/Article/details/gdyhhtsec.sHtML

[R12] for 遍历文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gctyjzapf.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gbyqqctsu.sHtML

[R13] for 计数循环
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gucfezscc.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gzxverglg.sHtML

[R14] C 风格 for
来源：http://baike.fanxiaobao.xyz/Article/details/gvjbxavgg.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gicwynvls.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfiekvytf.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvmkakacw.sHtML

[R16] until 等待条件
来源：http://blog.fanxiaobao.xyz/Article/details/gghhqpkgo.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.fanxiaobao.xyz/Article/details/gejnqxokr.sHtML

[R17] 数组定义与取值
来源：http://wap.fanxiaobao.xyz/Article/details/guomfuoje.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gmslifmog.sHtML

[R18] 遍历数组
来源：http://m.share.fanxiaobao.xyz/Article/details/gzzodoqyb.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.fanxiaobao.xyz/Article/details/ghinkpvpa.sHtML

[R19] 数组长度
来源：http://m.share.fanxiaobao.xyz/Article/details/gpprpchco.sHtML

echo "${#arr[@]}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gfowuqfkr.sHtML

[R20] 关联数组（字典）
来源：http://read.share.fanxiaobao.xyz/Article/details/gpzaxtuzi.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gpmudtcfu.sHtML

[R21] 字符串长度
来源：http://www.share.fanxiaobao.xyz/Article/details/giwdmvvco.sHtML

echo "${#s}"
来源：http://m.share.fanxiaobao.xyz/Article/details/ghygwthxw.sHtML

[R22] 截取子串
来源：http://mobile.fanxiaobao.xyz/Article/details/ghjsxtbgc.sHtML

echo "${s:0:5}"
来源：http://blog.fanxiaobao.xyz/Article/details/gtvdbiklh.sHtML

[R23] 字符串替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gtghuvikh.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gwmikazwd.sHtML

[R24] 大小写转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnnpitown.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.fanxiaobao.xyz/Article/details/gzuxiqlgw.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.fanxiaobao.xyz/Article/details/gbtoqwijd.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.fanxiaobao.xyz/Article/details/gzxmhxvry.sHtML

[R26] 命令替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gbiviufty.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqlwlorru.sHtML

[R27] 算术展开
来源：http://read.share.fanxiaobao.xyz/Article/details/gnmjanths.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.fanxiaobao.xyz/Article/details/gzeqciaif.sHtML

[R28] 浮点运算
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwyasvybv.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.fanxiaobao.xyz/Article/details/grkxppeod.sHtML

[R29] 定义函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gxcikpvwf.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/gswwuljxo.sHtML

[R30] 函数返回状态码
来源：http://blog.fanxiaobao.xyz/Article/details/geojeemlo.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.fanxiaobao.xyz/Article/details/gkvhicmyv.sHtML

[R31] 局部变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gvegvxljv.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.fanxiaobao.xyz/Article/details/gfzdjbehg.sHtML

[R32] 参数个数校验
来源：http://mobile.fanxiaobao.xyz/Article/details/gdjtiyeis.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.fanxiaobao.xyz/Article/details/gxolaxoof.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.fanxiaobao.xyz/Article/details/gildposky.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.fanxiaobao.xyz/Article/details/gzpunbhup.sHtML

[R34] 退出时清理
来源：http://blog.fanxiaobao.xyz/Article/details/gvcljzsdk.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.fanxiaobao.xyz/Article/details/gvuarpacv.sHtML

[R35] 后台执行并等待
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtaywihtw.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.fanxiaobao.xyz/Article/details/gbairfsby.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guswzslzk.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.fanxiaobao.xyz/Article/details/gkgqvlfxp.sHtML

[R37] 把输出赋给变量
来源：http://baike.fanxiaobao.xyz/Article/details/gmnqkbmtc.sHtML

files=$(ls -1)
来源：http://mobile.fanxiaobao.xyz/Article/details/glwiiglvt.sHtML

[R38] 管道串联
来源：http://www.blog.fanxiaobao.xyz/Article/details/grwnyoqif.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.fanxiaobao.xyz/Article/details/gkorxhxef.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.fanxiaobao.xyz/Article/details/gxdvyyshm.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gouyfumgy.sHtML

[R40] 追加写日志
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtsmekqvq.sHtML

echo "log" >> out.log
来源：http://3g.fanxiaobao.xyz/Article/details/glbypibdx.sHtML

[R41] 丢弃输出
来源：http://baike.fanxiaobao.xyz/Article/details/gcnmvlxqz.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.fanxiaobao.xyz/Article/details/ggksrzaax.sHtML

[R42] 输入重定向
来源：http://www.blog.fanxiaobao.xyz/Article/details/gekelzpce.sHtML

wc -l < a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/ggfryhzxg.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggrmashas.sHtML

find . -name "*.log" -type f
来源：http://m.share.fanxiaobao.xyz/Article/details/gjyvjutez.sHtML

[R44] 按修改时间查找
来源：http://3g.fanxiaobao.xyz/Article/details/guganwuca.sHtML

find . -mtime -7 -type f
来源：http://m.share.fanxiaobao.xyz/Article/details/gcjnhdgeh.sHtML

[R45] 批量删除
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcouzpvoz.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.fanxiaobao.xyz/Article/details/ghmupkkdi.sHtML

[R46] 递归替换文件内容
来源：http://blog.fanxiaobao.xyz/Article/details/grenbhyty.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.fanxiaobao.xyz/Article/details/gtnkwkjlx.sHtML

[R47] sed 单行替换
来源：http://www.share.fanxiaobao.xyz/Article/details/guwqsvlhv.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/grwzeeyde.sHtML

[R48] awk 取指定列
来源：http://3g.fanxiaobao.xyz/Article/details/gdtidgirx.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goquxmnuu.sHtML

[R49] awk 带条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gykgfbuak.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.fanxiaobao.xyz/Article/details/giymxblqp.sHtML

[R50] awk 求和
来源：http://baike.fanxiaobao.xyz/Article/details/gxsfewelb.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gueznlekm.sHtML

[R51] 排序去重取前几
来源：http://baike.fanxiaobao.xyz/Article/details/gyryvmkwc.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.fanxiaobao.xyz/Article/details/gbtfbmapl.sHtML

[R52] 统计行数
来源：http://blog.fanxiaobao.xyz/Article/details/gtjtmvhgt.sHtML

wc -l a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gjsutejuw.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghmxzzdwu.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsaszehrs.sHtML

[R54] 比较两个文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gsbggptsy.sHtML

diff a.txt b.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gduubcfpz.sHtML

[R55] 压缩与解压
来源：http://baike.fanxiaobao.xyz/Article/details/gpnggfrnq.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.fanxiaobao.xyz/Article/details/glsvjubnj.sHtML

[R56] 远程拷贝
来源：http://read.share.fanxiaobao.xyz/Article/details/godvoikax.sHtML

scp file user@host:/path/
来源：http://read.share.fanxiaobao.xyz/Article/details/gjzwdxoga.sHtML

[R57] 远程执行命令
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggcmnnbyi.sHtML

ssh user@host 'uptime'
来源：http://www.blog.fanxiaobao.xyz/Article/details/gynrkuwfk.sHtML

[R58] 下载文件
来源：http://blog.fanxiaobao.xyz/Article/details/gnwfvmqlq.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.fanxiaobao.xyz/Article/details/gldvppvtt.sHtML

[R59] 发 POST JSON
来源：http://blog.fanxiaobao.xyz/Article/details/gccroojpg.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.fanxiaobao.xyz/Article/details/grnkhulvf.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goqbgabti.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.fanxiaobao.xyz/Article/details/gkvaurfgh.sHtML

[R61] 磁盘占用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzlpfmroz.sHtML

df -h;  du -sh *
来源：http://wap.fanxiaobao.xyz/Article/details/gwsteokfr.sHtML

[R62] 找最占空间的文件
来源：http://mobile.fanxiaobao.xyz/Article/details/ggjqgtjrt.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkntkwxxc.sHtML

[R63] 内存与进程
来源：http://blog.fanxiaobao.xyz/Article/details/gnyxtimad.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.fanxiaobao.xyz/Article/details/gkwiiczrb.sHtML

[R64] 结束进程
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdncqakyb.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.fanxiaobao.xyz/Article/details/gdnpjstwm.sHtML

[R65] 查看端口占用
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzmggrdxm.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfrlwdkwj.sHtML

[R66] 定时任务
来源：http://blog.fanxiaobao.xyz/Article/details/gqckgagpe.sHtML

crontab -e;  crontab -l
来源：http://baike.fanxiaobao.xyz/Article/details/gvqxuejyu.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.fanxiaobao.xyz/Article/details/gswimwvch.sHtML

openssl rand -hex 16
来源：http://read.share.fanxiaobao.xyz/Article/details/gaisvfgxq.sHtML

[R68] 计算文件校验值
来源：http://www.share.fanxiaobao.xyz/Article/details/gndybohfv.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gazroyuls.sHtML

[R69] 生成随机密码
来源：http://read.share.fanxiaobao.xyz/Article/details/gxzavfpnt.sHtML

head -c 16 /dev/urandom | base64
来源：http://read.share.fanxiaobao.xyz/Article/details/gsxmxufgi.sHtML

[R70] 时间戳与互转
来源：http://blog.fanxiaobao.xyz/Article/details/gncwjmezu.sHtML

date +%s;  date -d @1700000000
来源：http://3g.fanxiaobao.xyz/Article/details/gpxnunzfs.sHtML

[R71] 日期格式化
来源：http://www.share.fanxiaobao.xyz/Article/details/gfebpyotg.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbjfpwrwm.sHtML

[R72] 等待端口就绪
来源：http://mobile.fanxiaobao.xyz/Article/details/gqndsltmw.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjwvjxmor.sHtML

[R73] 分割大日志
来源：http://m.share.fanxiaobao.xyz/Article/details/gyiruyoya.sHtML

split -l 1000 big.log part_
来源：http://www.share.fanxiaobao.xyz/Article/details/gugafiacp.sHtML

[R74] 批量重命名
来源：http://wap.fanxiaobao.xyz/Article/details/gqhjlcjrr.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gbwpvpabm.sHtML

[R75] 导出环境变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gjctqsyaw.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.fanxiaobao.xyz/Article/details/gezplygbb.sHtML

[R76] 使用临时文件
来源：http://3g.fanxiaobao.xyz/Article/details/gukedgolx.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmgkyallz.sHtML

[R77] 读取用户输入
来源：http://www.share.fanxiaobao.xyz/Article/details/gdcsaoajn.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnnptulgw.sHtML

[R78] 交互式菜单
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfixjjcjt.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.fanxiaobao.xyz/Article/details/gheubbcgr.sHtML

[R79] 解析命令行选项
来源：http://3g.fanxiaobao.xyz/Article/details/gvbkhmkwr.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.fanxiaobao.xyz/Article/details/ggdiukaio.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.fanxiaobao.xyz/Article/details/gxchqaltg.sHtML

time ./run.sh
来源：http://baike.fanxiaobao.xyz/Article/details/gwqjwjvvc.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gnorrbgdt.sHtML

S. C / C++ 专题
来源：http://mobile.fanxiaobao.xyz/Article/details/grsbrxnij.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyyggeran.sHtML

[S01] C：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gujtyfrhr.sHtML

#include <stdio.h>
来源：http://mobile.fanxiaobao.xyz/Article/details/gumrcsvay.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.fanxiaobao.xyz/Article/details/gyjtntbhl.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.fanxiaobao.xyz/Article/details/gowytbhbt.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.fanxiaobao.xyz/Article/details/gqhxjqrgr.sHtML

[S03] C：读入整数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gakicarpv.sHtML

int x; scanf("%d", &x);
来源：http://m.share.fanxiaobao.xyz/Article/details/gdgmtstkk.sHtML

[S04] C：字符串复制
来源：http://www.share.fanxiaobao.xyz/Article/details/gqpkrcwua.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guudjqrpe.sHtML

[S05] C：字符串长度
来源：http://mobile.fanxiaobao.xyz/Article/details/grbrkxwjv.sHtML

strlen(s)
来源：http://wap.fanxiaobao.xyz/Article/details/gizutbgtv.sHtML

[S06] C：字符串比较
来源：http://baike.fanxiaobao.xyz/Article/details/gaqlljcoc.sHtML

strcmp(a, b) == 0
来源：http://read.share.fanxiaobao.xyz/Article/details/gxdndopzs.sHtML

[S07] C：数组遍历求和
来源：http://wap.fanxiaobao.xyz/Article/details/gsgbyfzai.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.fanxiaobao.xyz/Article/details/gmhbxlpbm.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.fanxiaobao.xyz/Article/details/gkxrutxbf.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.fanxiaobao.xyz/Article/details/gjzhzrojk.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.fanxiaobao.xyz/Article/details/gknmcmjmv.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.fanxiaobao.xyz/Article/details/grphukqrf.sHtML

[S10] C：指针与解引用
来源：http://www.share.fanxiaobao.xyz/Article/details/gcgfyrqlo.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.fanxiaobao.xyz/Article/details/gctsfgioy.sHtML

[S11] C：逐行读文件
来源：http://3g.fanxiaobao.xyz/Article/details/gzlxqmzsh.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.fanxiaobao.xyz/Article/details/goroqvviu.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.fanxiaobao.xyz/Article/details/gxtwkyjlf.sHtML

fclose(f);
来源：http://mobile.fanxiaobao.xyz/Article/details/ghcewrtsd.sHtML

[S12] C：写文件
来源：http://blog.fanxiaobao.xyz/Article/details/gjgqxhkvi.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.fanxiaobao.xyz/Article/details/gjossshml.sHtML

[S13] C：宏定义
来源：http://wap.fanxiaobao.xyz/Article/details/gvmuznllc.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.fanxiaobao.xyz/Article/details/gxlgxnjxd.sHtML

[S14] C：枚举
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glzxjsfzj.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.fanxiaobao.xyz/Article/details/gynjifxep.sHtML

[S15] C：类型转换
来源：http://www.share.fanxiaobao.xyz/Article/details/gddbyfzwv.sHtML

(double) a / b
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnyljlysk.sHtML

[S16] C：位操作置位
来源：http://mobile.fanxiaobao.xyz/Article/details/gmppiycwj.sHtML

x |= (1 << 3);
来源：http://mobile.fanxiaobao.xyz/Article/details/gllazbgwg.sHtML

[S17] C：安全拼接字符串
来源：http://wap.fanxiaobao.xyz/Article/details/golnpdwei.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.fanxiaobao.xyz/Article/details/guudcqyjb.sHtML

[S18] C：命令行参数
来源：http://3g.fanxiaobao.xyz/Article/details/gjmzpbpsq.sHtML

int main(int argc, char **argv)
来源：http://mobile.fanxiaobao.xyz/Article/details/gawrsernx.sHtML

[S19] C：快速排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gshmeggma.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.fanxiaobao.xyz/Article/details/gukuedtoq.sHtML

[S20] C：二分查找
来源：http://read.share.fanxiaobao.xyz/Article/details/gbdqcefcd.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.fanxiaobao.xyz/Article/details/gxwgvfwxb.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfriqywar.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqopkczfi.sHtML

[S22] C：字符串转数字
来源：http://baike.fanxiaobao.xyz/Article/details/gzbjyrrke.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.fanxiaobao.xyz/Article/details/gxjkdnmyf.sHtML

[S23] C：随机数
来源：http://m.share.fanxiaobao.xyz/Article/details/gjtuwqlrt.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqddjovtm.sHtML

[S24] C：获取本地时间
来源：http://www.share.fanxiaobao.xyz/Article/details/gygwncknl.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.fanxiaobao.xyz/Article/details/gnkcrtmjr.sHtML

[S25] C：内存拷贝
来源：http://read.share.fanxiaobao.xyz/Article/details/gbswlrfkg.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjrncpmsr.sHtML

[S26] C：内存清零
来源：http://www.share.fanxiaobao.xyz/Article/details/gvbigdtqv.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.fanxiaobao.xyz/Article/details/gtfgxewua.sHtML

[S27] C：定义常量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbuufkpgy.sHtML

const double PI = 3.14159;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqogdmmix.sHtML

[S28] C：静态变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gmiwgwftd.sHtML

static int counter = 0;
来源：http://read.share.fanxiaobao.xyz/Article/details/gsletsfgx.sHtML

[S29] C：变参函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gybtphqko.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.fanxiaobao.xyz/Article/details/gvntfnwqn.sHtML

[S30] C：头文件保护
来源：http://mobile.fanxiaobao.xyz/Article/details/gtqyhbanj.sHtML

#ifndef X_H
来源：http://baike.fanxiaobao.xyz/Article/details/gndranvoh.sHtML

#define X_H
来源：http://3g.fanxiaobao.xyz/Article/details/gwniurwqp.sHtML

#endif
来源：http://mobile.fanxiaobao.xyz/Article/details/gbtceltbg.sHtML

[S31] C++：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/givzixaun.sHtML

#include <iostream>
来源：http://read.share.fanxiaobao.xyz/Article/details/gmzicxxww.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gkpzmrajf.sHtML

[S32] C++：字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/guvxcixwo.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.fanxiaobao.xyz/Article/details/gzgohjipo.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghbvfcxex.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.fanxiaobao.xyz/Article/details/gfzmbwwhx.sHtML

[S34] C++：遍历 vector
来源：http://wap.fanxiaobao.xyz/Article/details/gnayamfvx.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gfjsdgfls.sHtML

[S35] C++：map
来源：http://blog.fanxiaobao.xyz/Article/details/gexpnxjbt.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gbafznvtu.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gstucigma.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gyvfxlkvg.sHtML

[S37] C++：set
来源：http://m.share.fanxiaobao.xyz/Article/details/ggasyfrup.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.fanxiaobao.xyz/Article/details/gfktwbfsc.sHtML

[S38] C++：排序
来源：http://blog.fanxiaobao.xyz/Article/details/gdfftdhtt.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.fanxiaobao.xyz/Article/details/gbyobnoly.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.fanxiaobao.xyz/Article/details/gmyurpbwk.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.fanxiaobao.xyz/Article/details/gqoyldaka.sHtML

[S40] C++：查找元素
来源：http://blog.fanxiaobao.xyz/Article/details/gxdqbpixx.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grliesyeh.sHtML

[S41] C++：类与构造函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gzixqlfqt.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.fanxiaobao.xyz/Article/details/gpnxwkpxx.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gpooshnks.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.fanxiaobao.xyz/Article/details/gjpyupotc.sHtML

[S43] C++：智能指针
来源：http://read.share.fanxiaobao.xyz/Article/details/gspcqzayw.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.fanxiaobao.xyz/Article/details/gsnwpkygx.sHtML

[S44] C++：引用传参
来源：http://m.share.fanxiaobao.xyz/Article/details/glpdigynj.sHtML

void inc(int &x) { ++x; }
来源：http://wap.fanxiaobao.xyz/Article/details/getwlhdue.sHtML

[S45] C++：lambda
来源：http://m.share.fanxiaobao.xyz/Article/details/giyvcfgdm.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.fanxiaobao.xyz/Article/details/gynlaqonw.sHtML

[S46] C++：函数模板
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbwaaijfg.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gbltqtygm.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.fanxiaobao.xyz/Article/details/gluibhxmz.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.fanxiaobao.xyz/Article/details/gfovfyvek.sHtML

[S48] C++：逐行读文件
来源：http://baike.fanxiaobao.xyz/Article/details/gixuzsato.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqrjufeac.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.fanxiaobao.xyz/Article/details/gfmbcyygy.sHtML

[S49] C++：写文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gyuhiznki.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.fanxiaobao.xyz/Article/details/gvgqtmgpo.sHtML

[S50] C++：格式化数字
来源：http://mobile.fanxiaobao.xyz/Article/details/ggircrqgl.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.fanxiaobao.xyz/Article/details/gcyjojegl.sHtML

[S51] C++：显式类型转换
来源：http://read.share.fanxiaobao.xyz/Article/details/goopnjmnz.sHtML

static_cast<double>(a) / b
来源：http://wap.fanxiaobao.xyz/Article/details/gxswtlypy.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfzmbrned.sHtML

int size() const noexcept { return n_; }
来源：http://baike.fanxiaobao.xyz/Article/details/gtjgldzea.sHtML

[S53] C++：移动语义
来源：http://m.share.fanxiaobao.xyz/Article/details/gbkkujrls.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.fanxiaobao.xyz/Article/details/gngadpldy.sHtML

[S54] C++：异常处理
来源：http://www.blog.fanxiaobao.xyz/Article/details/glmqxtlvd.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.fanxiaobao.xyz/Article/details/gcijlcosn.sHtML

[S55] C++：结构化绑定
来源：http://baike.fanxiaobao.xyz/Article/details/gxpsggvnh.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.fanxiaobao.xyz/Article/details/gxjqxszfm.sHtML

[S56] C++：optional
来源：http://read.share.fanxiaobao.xyz/Article/details/gpgvzdaeh.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.fanxiaobao.xyz/Article/details/ghpzpturw.sHtML

[S57] C++：编译期常量
来源：http://baike.fanxiaobao.xyz/Article/details/gqdblqyew.sHtML

constexpr int N = 10;
来源：http://read.share.fanxiaobao.xyz/Article/details/gjeiwlekr.sHtML

[S58] C++：命名空间
来源：http://blog.fanxiaobao.xyz/Article/details/ghcsykbkq.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.fanxiaobao.xyz/Article/details/gdlmskjhi.sHtML

[S59] C++：静态断言
来源：http://wap.fanxiaobao.xyz/Article/details/gfrhqzslh.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.fanxiaobao.xyz/Article/details/getdenepb.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.fanxiaobao.xyz/Article/details/goxenyxks.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.fanxiaobao.xyz/Article/details/gjxpokfcz.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gnubzxxoy.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.fanxiaobao.xyz/Article/details/gvkwzerid.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/ghqqoieyv.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyxagktfr.sHtML

println("Hello")
来源：http://3g.fanxiaobao.xyz/Article/details/gwdagkqhg.sHtML

[T02] Kotlin：变量
来源：http://3g.fanxiaobao.xyz/Article/details/goscawprk.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghdqexyun.sHtML

[T03] Kotlin：字符串模板
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guedjdjge.sHtML

"值: $b"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gprochyit.sHtML

[T04] Kotlin：空安全
来源：http://m.share.fanxiaobao.xyz/Article/details/gxvoenbxr.sHtML

val n: String? = null;  n?.length
来源：http://www.share.fanxiaobao.xyz/Article/details/gimxenycn.sHtML

[T05] Kotlin：when 表达式
来源：http://wap.fanxiaobao.xyz/Article/details/gcsqdsiyx.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.fanxiaobao.xyz/Article/details/gnzsywrru.sHtML

[T06] Kotlin：集合映射
来源：http://blog.fanxiaobao.xyz/Article/details/glhqhumon.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://baike.fanxiaobao.xyz/Article/details/gxlwdaijs.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.fanxiaobao.xyz/Article/details/ghuprlsxt.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.fanxiaobao.xyz/Article/details/gafteyizp.sHtML

[T08] Kotlin：数据类
来源：http://3g.fanxiaobao.xyz/Article/details/gwpmfkxou.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.fanxiaobao.xyz/Article/details/gzsfnxmyo.sHtML


<!-- 参考信息 -->