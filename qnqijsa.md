代发 wailian999

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.zdbjq.cn/Article/details/gmstlzmcd.sHtML

[Q90] 生成序号列
来源：http://mobile.fehbvm.com/Article/details/gtdmjiwef.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.share.zdbjq.cn/Article/details/gdfeomkah.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gwdyiucsp.sHtML

R. Bash 专题
来源：http://read.share.hesvh.cn/Article/details/gevikugzq.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gahqttfmd.sHtML

[R01] shebang 与严格模式
来源：http://m.share.fehbvm.com/Article/details/ggwgomncb.sHtML

#!/usr/bin/env bash
来源：http://www.blog.hesvh.cn/Article/details/gyubwitnl.sHtML

set -euo pipefail
来源：http://read.share.fehbvm.com/Article/details/geysocljr.sHtML

[R02] 变量赋值与使用
来源：http://blog.hesvh.cn/Article/details/gcpezkeur.sHtML

name="Tom"; echo "$name"
来源：http://read.share.fehbvm.com/Article/details/gsfawrznw.sHtML

[R03] 只读变量
来源：http://www.share.zdbjq.cn/Article/details/gijghydsm.sHtML

readonly PI=3.14
来源：http://read.share.hesvh.cn/Article/details/gkxdjbtbc.sHtML

[R04] 位置参数
来源：http://m.share.fehbvm.com/Article/details/gxponuyjc.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.zdbjq.cn/Article/details/gtbntbski.sHtML

[R05] 参数默认值
来源：http://www.blog.hesvh.cn/Article/details/grinasjvm.sHtML

name="${1:-default}"
来源：http://www.blog.zdbjq.cn/Article/details/gokcpuvws.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.fehbvm.com/Article/details/gsgezaxih.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.fehbvm.com/Article/details/gkcfgwkym.sHtML

[R07] if 判断文件
来源：http://mobile.hesvh.cn/Article/details/gbpdtzroz.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.fehbvm.com/Article/details/gpdhpwnei.sHtML

[R08] 数值比较
来源：http://baike.zdbjq.cn/Article/details/gtglwfscu.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.hesvh.cn/Article/details/glunzkbok.sHtML

[R09] 字符串比较
来源：http://3g.fehbvm.com/Article/details/ggqeohmxg.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://3g.zdbjq.cn/Article/details/gxiuxsoxc.sHtML

[R10] 正则匹配
来源：http://www.m.share.hesvh.cn/Article/details/gajuhabbx.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://blog.fehbvm.com/Article/details/ghhzepzmi.sHtML

[R11] case 多分支
来源：http://read.share.hesvh.cn/Article/details/gmxbfhmey.sHtML

case "$1" in
来源：http://www.m.share.fehbvm.com/Article/details/gclhxduqs.sHtML

start) echo "启动" ;;
来源：http://www.blog.hesvh.cn/Article/details/goqwptjgs.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.hesvh.cn/Article/details/gfvchkmmf.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.zdbjq.cn/Article/details/gnhcghqif.sHtML

esac
来源：http://read.share.fehbvm.com/Article/details/gvlzkjjzm.sHtML

[R12] for 遍历文件
来源：http://blog.hesvh.cn/Article/details/gydfvsxjk.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.hesvh.cn/Article/details/guhoxkcmv.sHtML

[R13] for 计数循环
来源：http://wap.zdbjq.cn/Article/details/goenmcjjp.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.m.share.fehbvm.com/Article/details/gxkkwkngk.sHtML

[R14] C 风格 for
来源：http://www.blog.fehbvm.com/Article/details/gbdodvfiy.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://baike.hesvh.cn/Article/details/gaithtspo.sHtML

[R15] while 逐行读文件
来源：http://wap.zdbjq.cn/Article/details/grvybpihj.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.hesvh.cn/Article/details/grhlfssvj.sHtML

[R16] until 等待条件
来源：http://read.share.fehbvm.com/Article/details/gttymwdsp.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.hesvh.cn/Article/details/glgtqucgd.sHtML

[R17] 数组定义与取值
来源：http://wap.fehbvm.com/Article/details/gntrbyurb.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.zdbjq.cn/Article/details/gynosvkzz.sHtML

[R18] 遍历数组
来源：http://read.share.zdbjq.cn/Article/details/gyoqxoiea.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.zdbjq.cn/Article/details/girwdfwkj.sHtML

[R19] 数组长度
来源：http://mobile.zdbjq.cn/Article/details/gchhhykup.sHtML

echo "${#arr[@]}"
来源：http://3g.hesvh.cn/Article/details/gagjuhwiw.sHtML

[R20] 关联数组（字典）
来源：http://www.share.hesvh.cn/Article/details/gtpizotip.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.fehbvm.com/Article/details/gmtxgoeoy.sHtML

[R21] 字符串长度
来源：http://www.share.fehbvm.com/Article/details/gaqkvsirz.sHtML

echo "${#s}"
来源：http://www.blog.zdbjq.cn/Article/details/gobpnknkc.sHtML

[R22] 截取子串
来源：http://mobile.hesvh.cn/Article/details/gaghnfrbr.sHtML

echo "${s:0:5}"
来源：http://www.share.zdbjq.cn/Article/details/gwexbuidb.sHtML

[R23] 字符串替换
来源：http://www.blog.fehbvm.com/Article/details/gpfdpkxsv.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.fehbvm.com/Article/details/ghewqsrob.sHtML

[R24] 大小写转换
来源：http://mobile.fehbvm.com/Article/details/gicohuzup.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.fehbvm.com/Article/details/gefalmxgs.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.zdbjq.cn/Article/details/ghdxizvcp.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.zdbjq.cn/Article/details/geehcceyy.sHtML

[R26] 命令替换
来源：http://www.blog.hesvh.cn/Article/details/gomxipzhw.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.zdbjq.cn/Article/details/gymhlipwt.sHtML

[R27] 算术展开
来源：http://baike.hesvh.cn/Article/details/gvsqkihjs.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.fehbvm.com/Article/details/gqwjcivqq.sHtML

[R28] 浮点运算
来源：http://blog.zdbjq.cn/Article/details/gegyvongd.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.hesvh.cn/Article/details/gcvixwyvq.sHtML

[R29] 定义函数
来源：http://www.m.share.fehbvm.com/Article/details/gkczszpfp.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.hesvh.cn/Article/details/gyyivasiv.sHtML

[R30] 函数返回状态码
来源：http://read.share.fehbvm.com/Article/details/gzdmewpom.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.hesvh.cn/Article/details/ghiweinjg.sHtML

[R31] 局部变量
来源：http://m.share.zdbjq.cn/Article/details/gswnxrpqz.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.hesvh.cn/Article/details/giyovcokd.sHtML

[R32] 参数个数校验
来源：http://www.share.zdbjq.cn/Article/details/gzgbrlzfk.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.hesvh.cn/Article/details/gnhkzhrix.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.zdbjq.cn/Article/details/gkmpyhece.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.fehbvm.com/Article/details/gjxtcaqwu.sHtML

[R34] 退出时清理
来源：http://www.share.zdbjq.cn/Article/details/gdshkvutu.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.zdbjq.cn/Article/details/gmifikjfs.sHtML

[R35] 后台执行并等待
来源：http://read.share.zdbjq.cn/Article/details/gsamobfsj.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.hesvh.cn/Article/details/gmzkgcgtn.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.zdbjq.cn/Article/details/gztekqgua.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.hesvh.cn/Article/details/gfhnbxuii.sHtML

[R37] 把输出赋给变量
来源：http://m.share.fehbvm.com/Article/details/ggjvticra.sHtML

files=$(ls -1)
来源：http://www.m.share.fehbvm.com/Article/details/gurzeyeaw.sHtML

[R38] 管道串联
来源：http://mobile.fehbvm.com/Article/details/gsdzcjffw.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.hesvh.cn/Article/details/gmpmqizqt.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.fehbvm.com/Article/details/gxpoqlbew.sHtML

cmd > out.log 2>&1
来源：http://m.share.zdbjq.cn/Article/details/gidglpmth.sHtML

[R40] 追加写日志
来源：http://wap.hesvh.cn/Article/details/gabvmrlcn.sHtML

echo "log" >> out.log
来源：http://3g.fehbvm.com/Article/details/ghjbsgzuc.sHtML

[R41] 丢弃输出
来源：http://www.blog.fehbvm.com/Article/details/gxqhjffim.sHtML

cmd >/dev/null 2>&1
来源：http://mobile.fehbvm.com/Article/details/gatowyhqc.sHtML

[R42] 输入重定向
来源：http://blog.hesvh.cn/Article/details/gexwndnbb.sHtML

wc -l < a.txt
来源：http://www.share.zdbjq.cn/Article/details/gplfyjzxy.sHtML

[R43] 按名字查找文件
来源：http://3g.hesvh.cn/Article/details/gieajvram.sHtML

find . -name "*.log" -type f
来源：http://m.share.fehbvm.com/Article/details/guaeqzhvs.sHtML

[R44] 按修改时间查找
来源：http://www.share.zdbjq.cn/Article/details/gspqisrlm.sHtML

find . -mtime -7 -type f
来源：http://m.share.fehbvm.com/Article/details/gwldekkdl.sHtML

[R45] 批量删除
来源：http://read.share.fehbvm.com/Article/details/gjsgkrpyk.sHtML

find . -name "*.tmp" -delete
来源：http://baike.hesvh.cn/Article/details/goadtrrxe.sHtML

[R46] 递归替换文件内容
来源：http://wap.zdbjq.cn/Article/details/gftcwausf.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.zdbjq.cn/Article/details/gfddxbvhz.sHtML

[R47] sed 单行替换
来源：http://mobile.hesvh.cn/Article/details/gzgfuojdg.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.zdbjq.cn/Article/details/ghnekkpjr.sHtML

[R48] awk 取指定列
来源：http://www.m.share.hesvh.cn/Article/details/gyipkmmfl.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.fehbvm.com/Article/details/givhrawpf.sHtML

[R49] awk 带条件
来源：http://www.m.share.fehbvm.com/Article/details/gigommone.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.hesvh.cn/Article/details/gnyqdbgtw.sHtML

[R50] awk 求和
来源：http://read.share.fehbvm.com/Article/details/gsmjopsyi.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.hesvh.cn/Article/details/gkurdbchq.sHtML

[R51] 排序去重取前几
来源：http://wap.fehbvm.com/Article/details/glgkzcofu.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.zdbjq.cn/Article/details/gxdkqhdub.sHtML

[R52] 统计行数
来源：http://www.blog.fehbvm.com/Article/details/gaprqyvyg.sHtML

wc -l a.txt
来源：http://www.share.fehbvm.com/Article/details/gbxvgways.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.hesvh.cn/Article/details/gqameegyb.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.zdbjq.cn/Article/details/gwuhhjcgl.sHtML

[R54] 比较两个文件
来源：http://baike.hesvh.cn/Article/details/gmhgsetya.sHtML

diff a.txt b.txt
来源：http://read.share.fehbvm.com/Article/details/gaokwpklm.sHtML

[R55] 压缩与解压
来源：http://www.share.fehbvm.com/Article/details/gbhwlgnvm.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.hesvh.cn/Article/details/gnzhiksrb.sHtML

[R56] 远程拷贝
来源：http://3g.hesvh.cn/Article/details/gxpdgrfhu.sHtML

scp file user@host:/path/
来源：http://www.share.hesvh.cn/Article/details/gmfqcbxnn.sHtML

[R57] 远程执行命令
来源：http://read.share.fehbvm.com/Article/details/gfflrxzlf.sHtML

ssh user@host 'uptime'
来源：http://wap.zdbjq.cn/Article/details/grplraowr.sHtML

[R58] 下载文件
来源：http://blog.hesvh.cn/Article/details/gfanwnkov.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.zdbjq.cn/Article/details/gmpvrziyu.sHtML

[R59] 发 POST JSON
来源：http://3g.fehbvm.com/Article/details/gmlxinlkw.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.hesvh.cn/Article/details/gshimisht.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.zdbjq.cn/Article/details/gmtevqyfo.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.zdbjq.cn/Article/details/gexbziygc.sHtML

[R61] 磁盘占用
来源：http://m.share.fehbvm.com/Article/details/gssmvvalx.sHtML

df -h;  du -sh *
来源：http://read.share.hesvh.cn/Article/details/giyzbsrzq.sHtML

[R62] 找最占空间的文件
来源：http://3g.hesvh.cn/Article/details/gieqtesct.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.zdbjq.cn/Article/details/gzjclonch.sHtML

[R63] 内存与进程
来源：http://m.share.fehbvm.com/Article/details/grypiqmks.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.zdbjq.cn/Article/details/gricyqxlc.sHtML

[R64] 结束进程
来源：http://www.m.share.fehbvm.com/Article/details/guqroqccq.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.zdbjq.cn/Article/details/gqkusytsm.sHtML

[R65] 查看端口占用
来源：http://wap.fehbvm.com/Article/details/gseszjoty.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.hesvh.cn/Article/details/gbgbzvayu.sHtML

[R66] 定时任务
来源：http://www.share.fehbvm.com/Article/details/gskhheiyl.sHtML

crontab -e;  crontab -l
来源：http://3g.fehbvm.com/Article/details/gfpqdzrjk.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.fehbvm.com/Article/details/gbkvvngdd.sHtML

openssl rand -hex 16
来源：http://wap.zdbjq.cn/Article/details/gsuljzucm.sHtML

[R68] 计算文件校验值
来源：http://www.blog.zdbjq.cn/Article/details/gbcugclqn.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.fehbvm.com/Article/details/guxgnqnhb.sHtML

[R69] 生成随机密码
来源：http://blog.zdbjq.cn/Article/details/gygowktib.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.hesvh.cn/Article/details/gmicsidhz.sHtML

[R70] 时间戳与互转
来源：http://baike.hesvh.cn/Article/details/glieknxfw.sHtML

date +%s;  date -d @1700000000
来源：http://baike.fehbvm.com/Article/details/gzeaqpilu.sHtML

[R71] 日期格式化
来源：http://www.m.share.hesvh.cn/Article/details/gbkfferdb.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.hesvh.cn/Article/details/gytxjptfr.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.zdbjq.cn/Article/details/gggaxyzgj.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.fehbvm.com/Article/details/gkdpiadea.sHtML

[R73] 分割大日志
来源：http://www.blog.hesvh.cn/Article/details/gvkijwuum.sHtML

split -l 1000 big.log part_
来源：http://mobile.fehbvm.com/Article/details/goiilnepo.sHtML

[R74] 批量重命名
来源：http://mobile.hesvh.cn/Article/details/gbusrlfgx.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.zdbjq.cn/Article/details/gjspdcmtp.sHtML

[R75] 导出环境变量
来源：http://m.share.hesvh.cn/Article/details/gqkangekc.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.fehbvm.com/Article/details/gxqzvsktj.sHtML

[R76] 使用临时文件
来源：http://m.share.fehbvm.com/Article/details/gurelhzzp.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.fehbvm.com/Article/details/gimcjeucl.sHtML

[R77] 读取用户输入
来源：http://www.blog.zdbjq.cn/Article/details/gslefbcfh.sHtML

read -rp "请输入: " ans
来源：http://mobile.hesvh.cn/Article/details/gilpdaqqo.sHtML

[R78] 交互式菜单
来源：http://baike.zdbjq.cn/Article/details/gacolmbsa.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.zdbjq.cn/Article/details/gnwvrqcki.sHtML

[R79] 解析命令行选项
来源：http://3g.hesvh.cn/Article/details/gjxqumonb.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.zdbjq.cn/Article/details/gzwherkpe.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.hesvh.cn/Article/details/gnasemrka.sHtML

time ./run.sh
来源：http://3g.zdbjq.cn/Article/details/gigvspyda.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gtquamrfa.sHtML

S. C / C++ 专题
来源：http://wap.zdbjq.cn/Article/details/gstmcjfor.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gflbpqfkh.sHtML

[S01] C：Hello World
来源：http://3g.zdbjq.cn/Article/details/gejjpkibq.sHtML

#include <stdio.h>
来源：http://www.blog.zdbjq.cn/Article/details/gkblouwoz.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.zdbjq.cn/Article/details/grenblrod.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.hesvh.cn/Article/details/gylntxspg.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.zdbjq.cn/Article/details/gbqxqnalx.sHtML

[S03] C：读入整数
来源：http://3g.hesvh.cn/Article/details/gjwpykbqe.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.zdbjq.cn/Article/details/gwdrgoldj.sHtML

[S04] C：字符串复制
来源：http://3g.zdbjq.cn/Article/details/gcmmmjajo.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.fehbvm.com/Article/details/ghpatwpgq.sHtML

[S05] C：字符串长度
来源：http://www.m.share.fehbvm.com/Article/details/gdocgvaga.sHtML

strlen(s)
来源：http://www.share.hesvh.cn/Article/details/gzpxpyofw.sHtML

[S06] C：字符串比较
来源：http://blog.fehbvm.com/Article/details/gkqwtnhpv.sHtML

strcmp(a, b) == 0
来源：http://blog.hesvh.cn/Article/details/gvrnqasgu.sHtML

[S07] C：数组遍历求和
来源：http://www.share.zdbjq.cn/Article/details/gamfrnxnj.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.zdbjq.cn/Article/details/gcnifbyut.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.hesvh.cn/Article/details/gjtcamaew.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.hesvh.cn/Article/details/glrhjzrgj.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.hesvh.cn/Article/details/gewxzbiln.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.hesvh.cn/Article/details/gkagdpijb.sHtML

[S10] C：指针与解引用
来源：http://mobile.fehbvm.com/Article/details/gfjzcvltc.sHtML

int *p = &a;  *p = 5;
来源：http://3g.zdbjq.cn/Article/details/gkrgggzvs.sHtML

[S11] C：逐行读文件
来源：http://m.share.zdbjq.cn/Article/details/giaolujdc.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.zdbjq.cn/Article/details/gnbcrvvtz.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.fehbvm.com/Article/details/gsxaaqihr.sHtML

fclose(f);
来源：http://m.share.fehbvm.com/Article/details/gwqfuymhb.sHtML

[S12] C：写文件
来源：http://blog.hesvh.cn/Article/details/gvljfmqks.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.fehbvm.com/Article/details/golzzvgbs.sHtML

[S13] C：宏定义
来源：http://mobile.hesvh.cn/Article/details/glngajtiy.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.fehbvm.com/Article/details/gynjctxkt.sHtML

[S14] C：枚举
来源：http://www.blog.hesvh.cn/Article/details/gtcnwajzj.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.zdbjq.cn/Article/details/grxpppwoy.sHtML

[S15] C：类型转换
来源：http://3g.fehbvm.com/Article/details/gwjfzqeop.sHtML

(double) a / b
来源：http://baike.hesvh.cn/Article/details/gzkchrtyn.sHtML

[S16] C：位操作置位
来源：http://mobile.zdbjq.cn/Article/details/grlhkavce.sHtML

x |= (1 << 3);
来源：http://baike.hesvh.cn/Article/details/gagpuoiyz.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.zdbjq.cn/Article/details/gaaiwnmmb.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.hesvh.cn/Article/details/gqcqgcniv.sHtML

[S18] C：命令行参数
来源：http://blog.zdbjq.cn/Article/details/gchhiehip.sHtML

int main(int argc, char **argv)
来源：http://baike.fehbvm.com/Article/details/gctbuarzo.sHtML

[S19] C：快速排序
来源：http://baike.zdbjq.cn/Article/details/gxinfnbjq.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.fehbvm.com/Article/details/gqmdujmky.sHtML

[S20] C：二分查找
来源：http://www.share.zdbjq.cn/Article/details/gpcpybwtl.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.hesvh.cn/Article/details/ggokbicnm.sHtML

[S21] C：字符类别判断
来源：http://wap.fehbvm.com/Article/details/gigwaqmuo.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.zdbjq.cn/Article/details/gyjslfsdh.sHtML

[S22] C：字符串转数字
来源：http://read.share.zdbjq.cn/Article/details/ghyxpwuyb.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.zdbjq.cn/Article/details/gpjmnapbu.sHtML

[S23] C：随机数
来源：http://3g.fehbvm.com/Article/details/geczwlqoi.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.hesvh.cn/Article/details/gvosjflnz.sHtML

[S24] C：获取本地时间
来源：http://www.share.zdbjq.cn/Article/details/gfkhysnov.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.zdbjq.cn/Article/details/glbvtsksf.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.zdbjq.cn/Article/details/gnojrkdgk.sHtML

memcpy(dst, src, n);
来源：http://m.share.hesvh.cn/Article/details/guwqdaelw.sHtML

[S26] C：内存清零
来源：http://blog.hesvh.cn/Article/details/gwzktrkfd.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.hesvh.cn/Article/details/gkfptmbkn.sHtML

[S27] C：定义常量
来源：http://baike.hesvh.cn/Article/details/gxauyrqsf.sHtML

const double PI = 3.14159;
来源：http://www.share.fehbvm.com/Article/details/gjojnxuiz.sHtML

[S28] C：静态变量
来源：http://baike.hesvh.cn/Article/details/gpyznzmri.sHtML

static int counter = 0;
来源：http://wap.zdbjq.cn/Article/details/gecyuyjdp.sHtML

[S29] C：变参函数
来源：http://3g.zdbjq.cn/Article/details/gqzocsisk.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.zdbjq.cn/Article/details/gcujkttcu.sHtML

[S30] C：头文件保护
来源：http://blog.hesvh.cn/Article/details/gwaavnrbf.sHtML

#ifndef X_H
来源：http://baike.hesvh.cn/Article/details/gidckbqsv.sHtML

#define X_H
来源：http://blog.hesvh.cn/Article/details/ghpomsfcr.sHtML

#endif
来源：http://www.m.share.zdbjq.cn/Article/details/grosroafs.sHtML

[S31] C++：Hello World
来源：http://wap.fehbvm.com/Article/details/gghmbqwru.sHtML

#include <iostream>
来源：http://www.m.share.hesvh.cn/Article/details/gqqreirqm.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.fehbvm.com/Article/details/gymjbnobg.sHtML

[S32] C++：字符串
来源：http://3g.fehbvm.com/Article/details/gmzydnnqd.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.hesvh.cn/Article/details/gbcviqlow.sHtML

[S33] C++：vector 增删
来源：http://3g.fehbvm.com/Article/details/gzmeyrfzt.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.fehbvm.com/Article/details/gfzaddwsp.sHtML

[S34] C++：遍历 vector
来源：http://baike.hesvh.cn/Article/details/gnasmgjwn.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.zdbjq.cn/Article/details/gxtzenjoj.sHtML

[S35] C++：map
来源：http://www.m.share.hesvh.cn/Article/details/gmwrqmbqm.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.zdbjq.cn/Article/details/geqgehwda.sHtML

[S36] C++：unordered_map
来源：http://read.share.zdbjq.cn/Article/details/gohvjmpny.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.hesvh.cn/Article/details/gpypbxpsm.sHtML

[S37] C++：set
来源：http://mobile.fehbvm.com/Article/details/gwcsiawnx.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.zdbjq.cn/Article/details/gevhtcrom.sHtML

[S38] C++：排序
来源：http://3g.hesvh.cn/Article/details/gbahzyxfj.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.zdbjq.cn/Article/details/gdfpzvusq.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.hesvh.cn/Article/details/gbxcjgryv.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.fehbvm.com/Article/details/gxpnuqkkb.sHtML

[S40] C++：查找元素
来源：http://blog.fehbvm.com/Article/details/glnyilqup.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.zdbjq.cn/Article/details/gooywgfkt.sHtML

[S41] C++：类与构造函数
来源：http://m.share.zdbjq.cn/Article/details/gqptqhgzw.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.fehbvm.com/Article/details/gqqyrmawd.sHtML

[S42] C++：继承与虚函数
来源：http://wap.fehbvm.com/Article/details/ghxytnrou.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.hesvh.cn/Article/details/gbokvtoev.sHtML

[S43] C++：智能指针
来源：http://3g.zdbjq.cn/Article/details/gabzplxez.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.hesvh.cn/Article/details/grhbtjibe.sHtML

[S44] C++：引用传参
来源：http://www.share.hesvh.cn/Article/details/gezkjxejs.sHtML

void inc(int &x) { ++x; }
来源：http://baike.zdbjq.cn/Article/details/gjgqsavjx.sHtML

[S45] C++：lambda
来源：http://3g.hesvh.cn/Article/details/gthytzoso.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.zdbjq.cn/Article/details/greztpdez.sHtML

[S46] C++：函数模板
来源：http://www.m.share.zdbjq.cn/Article/details/gukrvdfrk.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.fehbvm.com/Article/details/gqmgyhukl.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.fehbvm.com/Article/details/ggsqdqbel.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.fehbvm.com/Article/details/gvvxbgmcv.sHtML

[S48] C++：逐行读文件
来源：http://wap.zdbjq.cn/Article/details/ganiaqmsp.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.zdbjq.cn/Article/details/gbtqdxqho.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.hesvh.cn/Article/details/gxklzmiis.sHtML

[S49] C++：写文件
来源：http://3g.hesvh.cn/Article/details/gkxlytplq.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.fehbvm.com/Article/details/gcinzpoon.sHtML

[S50] C++：格式化数字
来源：http://mobile.zdbjq.cn/Article/details/ggbqexjzi.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.zdbjq.cn/Article/details/gmeuxbzlj.sHtML

[S51] C++：显式类型转换
来源：http://mobile.zdbjq.cn/Article/details/gtuxppkwq.sHtML

static_cast<double>(a) / b
来源：http://www.blog.hesvh.cn/Article/details/gaaltiyvo.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.hesvh.cn/Article/details/goqbbhesj.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.hesvh.cn/Article/details/giintowzn.sHtML

[S53] C++：移动语义
来源：http://3g.zdbjq.cn/Article/details/gfujjrygz.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.zdbjq.cn/Article/details/gesmagffq.sHtML

[S54] C++：异常处理
来源：http://wap.fehbvm.com/Article/details/gctqnrpsg.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.zdbjq.cn/Article/details/gebigrmaq.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.hesvh.cn/Article/details/gliotmcma.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.fehbvm.com/Article/details/gzojvdbia.sHtML

[S56] C++：optional
来源：http://3g.hesvh.cn/Article/details/godnbidbm.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.hesvh.cn/Article/details/ggwsepffn.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.hesvh.cn/Article/details/gztmyzfbj.sHtML

constexpr int N = 10;
来源：http://3g.fehbvm.com/Article/details/gqsguydtn.sHtML

[S58] C++：命名空间
来源：http://mobile.fehbvm.com/Article/details/gxhwkkynx.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.zdbjq.cn/Article/details/gridtblpj.sHtML

[S59] C++：静态断言
来源：http://mobile.zdbjq.cn/Article/details/ggevxorxb.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.zdbjq.cn/Article/details/gehcesdwc.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.zdbjq.cn/Article/details/gbtzcafno.sHtML


<!-- 参考信息 -->