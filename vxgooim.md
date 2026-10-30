代发 wailian999

readonly PI=3.14
来源：http://www.share.zdbjq.cn/Article/details/gavgddqwu.sHtML

[R04] 位置参数
来源：http://www.share.zdbjq.cn/Article/details/gjwastxbc.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://m.share.zdbjq.cn/Article/details/gbfsvnxyk.sHtML

[R05] 参数默认值
来源：http://3g.fehbvm.com/Article/details/gkwmahkup.sHtML

name="${1:-default}"
来源：http://blog.zdbjq.cn/Article/details/gvqwswrzz.sHtML

[R06] 判断命令是否存在
来源：http://wap.fehbvm.com/Article/details/gdgdnoucr.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.zdbjq.cn/Article/details/ghcfukbdh.sHtML

[R07] if 判断文件
来源：http://wap.hesvh.cn/Article/details/gqhfbtpxx.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.fehbvm.com/Article/details/gmhikziud.sHtML

[R08] 数值比较
来源：http://blog.hesvh.cn/Article/details/gmeoqxfha.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.hesvh.cn/Article/details/genscttzx.sHtML

[R09] 字符串比较
来源：http://www.share.zdbjq.cn/Article/details/gigfjtbqc.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.fehbvm.com/Article/details/gtlfwvwdz.sHtML

[R10] 正则匹配
来源：http://read.share.fehbvm.com/Article/details/ghropfuut.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.zdbjq.cn/Article/details/gjloiyrfw.sHtML

[R11] case 多分支
来源：http://m.share.fehbvm.com/Article/details/gicqpukfa.sHtML

case "$1" in
来源：http://blog.zdbjq.cn/Article/details/gnvifaxqi.sHtML

start) echo "启动" ;;
来源：http://read.share.fehbvm.com/Article/details/gxwatyuof.sHtML

stop)  echo "停止" ;;
来源：http://wap.zdbjq.cn/Article/details/gvyxjrpqh.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.zdbjq.cn/Article/details/glomctpqd.sHtML

esac
来源：http://www.m.share.zdbjq.cn/Article/details/gcztmurww.sHtML

[R12] for 遍历文件
来源：http://www.share.fehbvm.com/Article/details/glvuoukor.sHtML

for f in *.txt; do echo "$f"; done
来源：http://mobile.fehbvm.com/Article/details/glphecvmr.sHtML

[R13] for 计数循环
来源：http://3g.fehbvm.com/Article/details/gbwtdpyjs.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.zdbjq.cn/Article/details/govyvnhin.sHtML

[R14] C 风格 for
来源：http://www.share.zdbjq.cn/Article/details/gnjixbcwp.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://baike.hesvh.cn/Article/details/gywbezjey.sHtML

[R15] while 逐行读文件
来源：http://baike.hesvh.cn/Article/details/gqmngutis.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.hesvh.cn/Article/details/glowvmyre.sHtML

[R16] until 等待条件
来源：http://www.blog.hesvh.cn/Article/details/gnytakzrr.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.fehbvm.com/Article/details/gqlcmkvwf.sHtML

[R17] 数组定义与取值
来源：http://read.share.zdbjq.cn/Article/details/gijbobjno.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.fehbvm.com/Article/details/gwwjtyuso.sHtML

[R18] 遍历数组
来源：http://www.m.share.fehbvm.com/Article/details/gxpducaki.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.share.zdbjq.cn/Article/details/gfsrgkkbf.sHtML

[R19] 数组长度
来源：http://mobile.zdbjq.cn/Article/details/gauoxgpaf.sHtML

echo "${#arr[@]}"
来源：http://m.share.fehbvm.com/Article/details/gkxilzyvx.sHtML

[R20] 关联数组（字典）
来源：http://wap.fehbvm.com/Article/details/gerbbpycf.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.fehbvm.com/Article/details/gfblfzcyd.sHtML

[R21] 字符串长度
来源：http://www.blog.hesvh.cn/Article/details/gjpfggbhg.sHtML

echo "${#s}"
来源：http://mobile.fehbvm.com/Article/details/guprhmtxm.sHtML

[R22] 截取子串
来源：http://www.blog.hesvh.cn/Article/details/gbrjiokje.sHtML

echo "${s:0:5}"
来源：http://read.share.hesvh.cn/Article/details/gopawgmvm.sHtML

[R23] 字符串替换
来源：http://3g.hesvh.cn/Article/details/gnxaskmjv.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.fehbvm.com/Article/details/gzckgkppl.sHtML

[R24] 大小写转换
来源：http://mobile.hesvh.cn/Article/details/gjwlpwhan.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.fehbvm.com/Article/details/gfypyklaw.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.fehbvm.com/Article/details/gnakgrcpn.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.hesvh.cn/Article/details/gzaigeqgh.sHtML

[R26] 命令替换
来源：http://read.share.fehbvm.com/Article/details/ghtzivckl.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.fehbvm.com/Article/details/gtrzzqdse.sHtML

[R27] 算术展开
来源：http://www.blog.fehbvm.com/Article/details/gwzsutuqk.sHtML

echo $((1 + 2 * 3))
来源：http://3g.hesvh.cn/Article/details/gfpaerjng.sHtML

[R28] 浮点运算
来源：http://3g.hesvh.cn/Article/details/gwxunxjyu.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.fehbvm.com/Article/details/gjrrkplng.sHtML

[R29] 定义函数
来源：http://blog.fehbvm.com/Article/details/grlvplfva.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.zdbjq.cn/Article/details/gmfbavkmo.sHtML

[R30] 函数返回状态码
来源：http://wap.zdbjq.cn/Article/details/gbndehupm.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.hesvh.cn/Article/details/gnqpuxceg.sHtML

[R31] 局部变量
来源：http://read.share.fehbvm.com/Article/details/grspmsxdz.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.hesvh.cn/Article/details/gqhltciat.sHtML

[R32] 参数个数校验
来源：http://baike.fehbvm.com/Article/details/ghsevhjeu.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.hesvh.cn/Article/details/gwuiwsnoz.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.fehbvm.com/Article/details/gdyioxjph.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.hesvh.cn/Article/details/ggbqrkstp.sHtML

[R34] 退出时清理
来源：http://wap.fehbvm.com/Article/details/gauxitzns.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.hesvh.cn/Article/details/gsadvqezd.sHtML

[R35] 后台执行并等待
来源：http://m.share.hesvh.cn/Article/details/gtkyorudu.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.fehbvm.com/Article/details/gbmuldplx.sHtML

[R36] 并发执行多个任务
来源：http://mobile.fehbvm.com/Article/details/geeziypzl.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.fehbvm.com/Article/details/gdcrihzdm.sHtML

[R37] 把输出赋给变量
来源：http://blog.hesvh.cn/Article/details/ggsphkkup.sHtML

files=$(ls -1)
来源：http://baike.zdbjq.cn/Article/details/gktsubdgu.sHtML

[R38] 管道串联
来源：http://3g.zdbjq.cn/Article/details/guwntnreq.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.zdbjq.cn/Article/details/gxhdrypsg.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.fehbvm.com/Article/details/glfflukmt.sHtML

cmd > out.log 2>&1
来源：http://mobile.zdbjq.cn/Article/details/gbtsvvhgm.sHtML

[R40] 追加写日志
来源：http://mobile.fehbvm.com/Article/details/gnqjusams.sHtML

echo "log" >> out.log
来源：http://blog.hesvh.cn/Article/details/gpvpiczzh.sHtML

[R41] 丢弃输出
来源：http://3g.fehbvm.com/Article/details/glenhsmwx.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.hesvh.cn/Article/details/gbcmciokv.sHtML

[R42] 输入重定向
来源：http://mobile.zdbjq.cn/Article/details/gqhjssnrs.sHtML

wc -l < a.txt
来源：http://blog.zdbjq.cn/Article/details/gqqaxdaea.sHtML

[R43] 按名字查找文件
来源：http://www.share.zdbjq.cn/Article/details/goxvlmayl.sHtML

find . -name "*.log" -type f
来源：http://3g.zdbjq.cn/Article/details/ggxbovisb.sHtML

[R44] 按修改时间查找
来源：http://read.share.zdbjq.cn/Article/details/ginmgvwdx.sHtML

find . -mtime -7 -type f
来源：http://3g.zdbjq.cn/Article/details/ghyebfvtg.sHtML

[R45] 批量删除
来源：http://m.share.zdbjq.cn/Article/details/grjaqcuey.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.zdbjq.cn/Article/details/giizalzux.sHtML

[R46] 递归替换文件内容
来源：http://blog.zdbjq.cn/Article/details/gvyepydzc.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://m.share.zdbjq.cn/Article/details/ghlbvqpsj.sHtML

[R47] sed 单行替换
来源：http://wap.zdbjq.cn/Article/details/gnjajcovb.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.zdbjq.cn/Article/details/gokyvhlxw.sHtML

[R48] awk 取指定列
来源：http://read.share.fehbvm.com/Article/details/gegttchgk.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.hesvh.cn/Article/details/ghsjszkaz.sHtML

[R49] awk 带条件
来源：http://read.share.fehbvm.com/Article/details/ggpviuxov.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.zdbjq.cn/Article/details/gtzswxwpj.sHtML

[R50] awk 求和
来源：http://baike.zdbjq.cn/Article/details/godlrtajm.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.fehbvm.com/Article/details/gufvxmkzv.sHtML

[R51] 排序去重取前几
来源：http://www.blog.zdbjq.cn/Article/details/gdnxrsiqo.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.zdbjq.cn/Article/details/gjvfqvfxz.sHtML

[R52] 统计行数
来源：http://read.share.hesvh.cn/Article/details/gcwtdtqjx.sHtML

wc -l a.txt
来源：http://www.blog.fehbvm.com/Article/details/gprlbxehd.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.fehbvm.com/Article/details/gmfmnxcoa.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.fehbvm.com/Article/details/gyrqoqofo.sHtML

[R54] 比较两个文件
来源：http://baike.hesvh.cn/Article/details/gmqazrvfr.sHtML

diff a.txt b.txt
来源：http://www.blog.hesvh.cn/Article/details/gwjorqyot.sHtML

[R55] 压缩与解压
来源：http://wap.hesvh.cn/Article/details/guheiuiyc.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.fehbvm.com/Article/details/gmkycdmxx.sHtML

[R56] 远程拷贝
来源：http://www.m.share.fehbvm.com/Article/details/gzhakylnb.sHtML

scp file user@host:/path/
来源：http://baike.zdbjq.cn/Article/details/gdmihbgbd.sHtML

[R57] 远程执行命令
来源：http://www.m.share.zdbjq.cn/Article/details/gfjtjgdkx.sHtML

ssh user@host 'uptime'
来源：http://www.share.hesvh.cn/Article/details/gbskedwog.sHtML

[R58] 下载文件
来源：http://www.share.zdbjq.cn/Article/details/gizubekil.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.hesvh.cn/Article/details/gogadwykt.sHtML

[R59] 发 POST JSON
来源：http://baike.zdbjq.cn/Article/details/gixxfyhsx.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.zdbjq.cn/Article/details/ggwwkmhyi.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.fehbvm.com/Article/details/guayibhfj.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.hesvh.cn/Article/details/gspfeteno.sHtML

[R61] 磁盘占用
来源：http://www.blog.hesvh.cn/Article/details/gyzmsyopd.sHtML

df -h;  du -sh *
来源：http://3g.fehbvm.com/Article/details/gzjnowupj.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.fehbvm.com/Article/details/gqrbloorb.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.zdbjq.cn/Article/details/gdrwdzehz.sHtML

[R63] 内存与进程
来源：http://www.blog.hesvh.cn/Article/details/gpmwincli.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.hesvh.cn/Article/details/gnaksecmr.sHtML

[R64] 结束进程
来源：http://wap.hesvh.cn/Article/details/gpyatujdd.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.hesvh.cn/Article/details/gtldvhwfw.sHtML

[R65] 查看端口占用
来源：http://blog.hesvh.cn/Article/details/gvxiduldu.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.hesvh.cn/Article/details/gfkoxxkfz.sHtML

[R66] 定时任务
来源：http://baike.hesvh.cn/Article/details/gywqgzpjg.sHtML

crontab -e;  crontab -l
来源：http://www.share.fehbvm.com/Article/details/gbmrjydsp.sHtML

[R67] 生成随机十六进制串
来源：http://baike.hesvh.cn/Article/details/gjpylcxja.sHtML

openssl rand -hex 16
来源：http://www.m.share.zdbjq.cn/Article/details/gperyfjui.sHtML

[R68] 计算文件校验值
来源：http://blog.fehbvm.com/Article/details/ggrnzbexi.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.hesvh.cn/Article/details/gdtyowfuy.sHtML

[R69] 生成随机密码
来源：http://www.m.share.zdbjq.cn/Article/details/gcnehrcdp.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.hesvh.cn/Article/details/gnqgusjpm.sHtML

[R70] 时间戳与互转
来源：http://m.share.zdbjq.cn/Article/details/grjiwrglf.sHtML

date +%s;  date -d @1700000000
来源：http://baike.hesvh.cn/Article/details/gvjtsvykh.sHtML

[R71] 日期格式化
来源：http://read.share.zdbjq.cn/Article/details/guhzideuw.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.zdbjq.cn/Article/details/girtojhvq.sHtML

[R72] 等待端口就绪
来源：http://mobile.hesvh.cn/Article/details/glihcwzyc.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.zdbjq.cn/Article/details/gpbkwbpsx.sHtML

[R73] 分割大日志
来源：http://3g.zdbjq.cn/Article/details/ggutpwjav.sHtML

split -l 1000 big.log part_
来源：http://baike.fehbvm.com/Article/details/gdxxhzpqu.sHtML

[R74] 批量重命名
来源：http://mobile.hesvh.cn/Article/details/glrnatmwd.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.zdbjq.cn/Article/details/gsrpmqupn.sHtML

[R75] 导出环境变量
来源：http://blog.zdbjq.cn/Article/details/gkzcnwhkj.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.fehbvm.com/Article/details/gjmmvopzl.sHtML

[R76] 使用临时文件
来源：http://wap.zdbjq.cn/Article/details/ghfmwbirf.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.zdbjq.cn/Article/details/gbmsuzeta.sHtML

[R77] 读取用户输入
来源：http://blog.zdbjq.cn/Article/details/gnjqadlmj.sHtML

read -rp "请输入: " ans
来源：http://baike.fehbvm.com/Article/details/gesbjqvlw.sHtML

[R78] 交互式菜单
来源：http://baike.zdbjq.cn/Article/details/ghgmgscko.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.fehbvm.com/Article/details/gqazhmjhc.sHtML

[R79] 解析命令行选项
来源：http://www.share.zdbjq.cn/Article/details/gfndbmlqz.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.zdbjq.cn/Article/details/gorimndvo.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.hesvh.cn/Article/details/gpetxwksj.sHtML

time ./run.sh
来源：http://3g.zdbjq.cn/Article/details/gwwrfjrgu.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/ggzbsmywz.sHtML

S. C / C++ 专题
来源：http://blog.zdbjq.cn/Article/details/gqivbegmi.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gbfduikrs.sHtML

[S01] C：Hello World
来源：http://3g.fehbvm.com/Article/details/gavkrviit.sHtML

#include <stdio.h>
来源：http://www.share.zdbjq.cn/Article/details/gssyysjww.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.hesvh.cn/Article/details/guoqqbker.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.hesvh.cn/Article/details/gnuflsttz.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.fehbvm.com/Article/details/gtejsfiva.sHtML

[S03] C：读入整数
来源：http://blog.hesvh.cn/Article/details/gwkhpqgjb.sHtML

int x; scanf("%d", &x);
来源：http://wap.zdbjq.cn/Article/details/gsjhkxqes.sHtML

[S04] C：字符串复制
来源：http://blog.fehbvm.com/Article/details/gesjrsajq.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.hesvh.cn/Article/details/gsdcejuth.sHtML

[S05] C：字符串长度
来源：http://3g.zdbjq.cn/Article/details/gatyggtgm.sHtML

strlen(s)
来源：http://www.blog.fehbvm.com/Article/details/ggdgwzivy.sHtML

[S06] C：字符串比较
来源：http://blog.zdbjq.cn/Article/details/gdgxzexwv.sHtML

strcmp(a, b) == 0
来源：http://3g.hesvh.cn/Article/details/goxvneafk.sHtML

[S07] C：数组遍历求和
来源：http://wap.fehbvm.com/Article/details/gpofclprr.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.hesvh.cn/Article/details/gtocnzcpp.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.zdbjq.cn/Article/details/ghehafabo.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.hesvh.cn/Article/details/gnajeiwwe.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.zdbjq.cn/Article/details/gujqluvmj.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.hesvh.cn/Article/details/gzvaxjxjw.sHtML

[S10] C：指针与解引用
来源：http://www.share.zdbjq.cn/Article/details/gmwvcyrql.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.zdbjq.cn/Article/details/gugfooufy.sHtML

[S11] C：逐行读文件
来源：http://read.share.hesvh.cn/Article/details/gqvwlhwbs.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.fehbvm.com/Article/details/gyriszfjl.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.zdbjq.cn/Article/details/gaypxmbmi.sHtML

fclose(f);
来源：http://m.share.hesvh.cn/Article/details/gzfrrazir.sHtML

[S12] C：写文件
来源：http://blog.zdbjq.cn/Article/details/gvhqquqga.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.zdbjq.cn/Article/details/gubquaact.sHtML

[S13] C：宏定义
来源：http://www.m.share.zdbjq.cn/Article/details/gkqghuujb.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.hesvh.cn/Article/details/gxbioyjso.sHtML

[S14] C：枚举
来源：http://www.blog.hesvh.cn/Article/details/gxgftdoyy.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.zdbjq.cn/Article/details/gygwozxfq.sHtML

[S15] C：类型转换
来源：http://www.m.share.hesvh.cn/Article/details/guphseepi.sHtML

(double) a / b
来源：http://www.share.hesvh.cn/Article/details/ggpxbnibb.sHtML

[S16] C：位操作置位
来源：http://wap.fehbvm.com/Article/details/gmpzaectn.sHtML

x |= (1 << 3);
来源：http://read.share.zdbjq.cn/Article/details/gqyffieob.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.fehbvm.com/Article/details/gaxhtevhk.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.hesvh.cn/Article/details/glhrzwtuz.sHtML

[S18] C：命令行参数
来源：http://3g.hesvh.cn/Article/details/gljsntjmi.sHtML

int main(int argc, char **argv)
来源：http://read.share.hesvh.cn/Article/details/gpcwpjasw.sHtML

[S19] C：快速排序
来源：http://3g.zdbjq.cn/Article/details/gpkancoxm.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.hesvh.cn/Article/details/gbjgfiogl.sHtML

[S20] C：二分查找
来源：http://3g.zdbjq.cn/Article/details/gqaibuqtc.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.hesvh.cn/Article/details/genirhwgh.sHtML

[S21] C：字符类别判断
来源：http://wap.zdbjq.cn/Article/details/gklhrhaii.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.hesvh.cn/Article/details/gjmabiiqr.sHtML

[S22] C：字符串转数字
来源：http://blog.fehbvm.com/Article/details/gyxxazyec.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.fehbvm.com/Article/details/gxwonvuwo.sHtML

[S23] C：随机数
来源：http://mobile.zdbjq.cn/Article/details/gbbeifskx.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.zdbjq.cn/Article/details/gsktuggkw.sHtML

[S24] C：获取本地时间
来源：http://read.share.hesvh.cn/Article/details/goytithgu.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.fehbvm.com/Article/details/gmvziejdj.sHtML

[S25] C：内存拷贝
来源：http://read.share.fehbvm.com/Article/details/gesvxwhvn.sHtML

memcpy(dst, src, n);
来源：http://wap.zdbjq.cn/Article/details/gnhiwhjsb.sHtML

[S26] C：内存清零
来源：http://read.share.zdbjq.cn/Article/details/gexdoxxii.sHtML

memset(a, 0, sizeof a);
来源：http://3g.fehbvm.com/Article/details/gadeniyfm.sHtML

[S27] C：定义常量
来源：http://baike.fehbvm.com/Article/details/gwwdaiquu.sHtML

const double PI = 3.14159;
来源：http://www.share.fehbvm.com/Article/details/gofrksizt.sHtML

[S28] C：静态变量
来源：http://blog.zdbjq.cn/Article/details/gzlodcvnt.sHtML

static int counter = 0;
来源：http://mobile.zdbjq.cn/Article/details/gmffvbors.sHtML

[S29] C：变参函数
来源：http://www.m.share.hesvh.cn/Article/details/gitfokmkr.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.fehbvm.com/Article/details/goopvxehw.sHtML

[S30] C：头文件保护
来源：http://3g.hesvh.cn/Article/details/gjfefferp.sHtML

#ifndef X_H
来源：http://3g.hesvh.cn/Article/details/gucnscjal.sHtML

#define X_H
来源：http://blog.hesvh.cn/Article/details/gqqeakftt.sHtML

#endif
来源：http://read.share.hesvh.cn/Article/details/gzrsgutaj.sHtML

[S31] C++：Hello World
来源：http://www.blog.fehbvm.com/Article/details/gsoywtfrc.sHtML

#include <iostream>
来源：http://www.blog.fehbvm.com/Article/details/gtvwzhrsz.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.zdbjq.cn/Article/details/gbamwlpwt.sHtML

[S32] C++：字符串
来源：http://3g.zdbjq.cn/Article/details/gwkfbhgcm.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.hesvh.cn/Article/details/gmvsmycfv.sHtML

[S33] C++：vector 增删
来源：http://read.share.hesvh.cn/Article/details/grbgpqhwm.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.zdbjq.cn/Article/details/gigrxueuz.sHtML

[S34] C++：遍历 vector
来源：http://blog.hesvh.cn/Article/details/gfeoupkme.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.hesvh.cn/Article/details/gkmmjwudp.sHtML

[S35] C++：map
来源：http://www.share.fehbvm.com/Article/details/glareufqx.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.hesvh.cn/Article/details/gseywdthf.sHtML

[S36] C++：unordered_map
来源：http://blog.zdbjq.cn/Article/details/gonfhmbju.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.fehbvm.com/Article/details/getpqcjoq.sHtML

[S37] C++：set
来源：http://www.share.zdbjq.cn/Article/details/gntxififi.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.hesvh.cn/Article/details/gcetokrfh.sHtML

[S38] C++：排序
来源：http://3g.fehbvm.com/Article/details/gcgnjzfuj.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.fehbvm.com/Article/details/gyzjmyuav.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.zdbjq.cn/Article/details/gumnwrkdj.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.fehbvm.com/Article/details/gklvtiltf.sHtML

[S40] C++：查找元素
来源：http://blog.zdbjq.cn/Article/details/gaoyjcqji.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.zdbjq.cn/Article/details/gfbvgpuzq.sHtML

[S41] C++：类与构造函数
来源：http://blog.hesvh.cn/Article/details/gmyjouspq.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.zdbjq.cn/Article/details/gwqvgzotg.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.hesvh.cn/Article/details/grrrtcief.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.m.share.hesvh.cn/Article/details/gtjcubjzm.sHtML

[S43] C++：智能指针
来源：http://baike.fehbvm.com/Article/details/ggwqkcbwx.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.hesvh.cn/Article/details/gcjohpype.sHtML

[S44] C++：引用传参
来源：http://www.m.share.hesvh.cn/Article/details/gkknskuhj.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.hesvh.cn/Article/details/ghokhiodf.sHtML

[S45] C++：lambda
来源：http://3g.hesvh.cn/Article/details/gvvowsozy.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.zdbjq.cn/Article/details/guxguslga.sHtML

[S46] C++：函数模板
来源：http://3g.zdbjq.cn/Article/details/gqkeasqof.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.zdbjq.cn/Article/details/gioetigia.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.zdbjq.cn/Article/details/gdzasppxt.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.hesvh.cn/Article/details/gorfusdpn.sHtML

[S48] C++：逐行读文件
来源：http://wap.zdbjq.cn/Article/details/gzfkndwfx.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.zdbjq.cn/Article/details/gvdegxago.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.hesvh.cn/Article/details/ggseytlqh.sHtML

[S49] C++：写文件
来源：http://blog.fehbvm.com/Article/details/gqbnryjnz.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.fehbvm.com/Article/details/gvlqttisl.sHtML

[S50] C++：格式化数字
来源：http://3g.zdbjq.cn/Article/details/ghzhkeekl.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.zdbjq.cn/Article/details/gjnemhjkk.sHtML

[S51] C++：显式类型转换
来源：http://wap.hesvh.cn/Article/details/gcceizdcf.sHtML

static_cast<double>(a) / b
来源：http://baike.zdbjq.cn/Article/details/gsnnphiyt.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.hesvh.cn/Article/details/gzuxrwtkp.sHtML

int size() const noexcept { return n_; }
来源：http://3g.hesvh.cn/Article/details/gvkoyjvqa.sHtML

[S53] C++：移动语义
来源：http://www.share.hesvh.cn/Article/details/gtnogfinb.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.fehbvm.com/Article/details/gvcfbozgp.sHtML

[S54] C++：异常处理
来源：http://3g.zdbjq.cn/Article/details/gruyaahbj.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.zdbjq.cn/Article/details/gvdligcsi.sHtML

[S55] C++：结构化绑定
来源：http://read.share.fehbvm.com/Article/details/gsyiueuzu.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.zdbjq.cn/Article/details/gcubqorei.sHtML

[S56] C++：optional
来源：http://wap.zdbjq.cn/Article/details/gsufuxbug.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.hesvh.cn/Article/details/gntptovjh.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.zdbjq.cn/Article/details/ggbmduoom.sHtML

constexpr int N = 10;
来源：http://baike.fehbvm.com/Article/details/gtfdbvrud.sHtML

[S58] C++：命名空间
来源：http://www.m.share.hesvh.cn/Article/details/gqhnlccvz.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.zdbjq.cn/Article/details/gtjgtbmng.sHtML

[S59] C++：静态断言
来源：http://m.share.fehbvm.com/Article/details/gcqybqwxr.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.hesvh.cn/Article/details/gfluomwel.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.zdbjq.cn/Article/details/gwtxcqnjf.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.fehbvm.com/Article/details/gukjftaxc.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gszboitsv.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.hesvh.cn/Article/details/gvokrundq.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gtovefiip.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.hesvh.cn/Article/details/gnrrurofh.sHtML

println("Hello")
来源：http://www.blog.fehbvm.com/Article/details/ggaismoqw.sHtML

[T02] Kotlin：变量
来源：http://mobile.fehbvm.com/Article/details/gmqtlhjzw.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.zdbjq.cn/Article/details/gwazusqus.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.zdbjq.cn/Article/details/gvccvvqqk.sHtML

"值: $b"
来源：http://3g.zdbjq.cn/Article/details/glzmvnemn.sHtML

[T04] Kotlin：空安全
来源：http://www.share.fehbvm.com/Article/details/gfamvpqgq.sHtML

val n: String? = null;  n?.length
来源：http://baike.zdbjq.cn/Article/details/gwrkryzta.sHtML


<!-- 参考信息 -->