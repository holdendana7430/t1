代发 wailian999

[Q86] 读取 JSON 字段
来源：http://www.blog.zdbjq.cn/Article/details/gmbduxotv.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://blog.zdbjq.cn/Article/details/gvdvxurjl.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.hesvh.cn/Article/details/gsvxsngmy.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.m.share.zdbjq.cn/Article/details/gjtajdwjf.sHtML

[Q88] 行转列（条件聚合）
来源：http://m.share.hesvh.cn/Article/details/gdboaxifn.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.share.hesvh.cn/Article/details/gkajwzlpr.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mobile.fehbvm.com/Article/details/gldwxvggy.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.fehbvm.com/Article/details/glenjmwxl.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wap.hesvh.cn/Article/details/gywvnnnrp.sHtML

[Q90] 生成序号列
来源：http://blog.fehbvm.com/Article/details/gntyuntzm.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://baike.fehbvm.com/Article/details/gjkdlnlsd.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gxthfmcnv.sHtML

R. Bash 专题
来源：http://mobile.hesvh.cn/Article/details/gyundslls.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gmbfghhil.sHtML

[R01] shebang 与严格模式
来源：http://www.share.fehbvm.com/Article/details/gmkveambx.sHtML

#!/usr/bin/env bash
来源：http://wap.hesvh.cn/Article/details/ggsdggoee.sHtML

set -euo pipefail
来源：http://mobile.zdbjq.cn/Article/details/gtwjxcabs.sHtML

[R02] 变量赋值与使用
来源：http://www.blog.fehbvm.com/Article/details/gbpcgxjxu.sHtML

name="Tom"; echo "$name"
来源：http://wap.hesvh.cn/Article/details/ginyvahym.sHtML

[R03] 只读变量
来源：http://www.share.fehbvm.com/Article/details/ggapahanf.sHtML

readonly PI=3.14
来源：http://blog.fehbvm.com/Article/details/gluldyvyu.sHtML

[R04] 位置参数
来源：http://www.share.hesvh.cn/Article/details/gyldwdnjy.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.fehbvm.com/Article/details/gvsgsojwm.sHtML

[R05] 参数默认值
来源：http://www.share.hesvh.cn/Article/details/gysqvmqhj.sHtML

name="${1:-default}"
来源：http://www.blog.hesvh.cn/Article/details/gsqdlyawk.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.fehbvm.com/Article/details/gvehfwcbk.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.zdbjq.cn/Article/details/gayimpqjw.sHtML

[R07] if 判断文件
来源：http://www.blog.hesvh.cn/Article/details/gjvapikcx.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.zdbjq.cn/Article/details/gcvvuetje.sHtML

[R08] 数值比较
来源：http://www.blog.zdbjq.cn/Article/details/gkapsbmfq.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://m.share.hesvh.cn/Article/details/gpfzyreuj.sHtML

[R09] 字符串比较
来源：http://wap.zdbjq.cn/Article/details/gcmhgazgx.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.zdbjq.cn/Article/details/gzhcsuyan.sHtML

[R10] 正则匹配
来源：http://baike.zdbjq.cn/Article/details/gafohltey.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.fehbvm.com/Article/details/gcqopdpyy.sHtML

[R11] case 多分支
来源：http://wap.fehbvm.com/Article/details/gyjbevzcd.sHtML

case "$1" in
来源：http://wap.hesvh.cn/Article/details/gdhpbdwqm.sHtML

start) echo "启动" ;;
来源：http://www.share.hesvh.cn/Article/details/gldpfyrcj.sHtML

stop)  echo "停止" ;;
来源：http://read.share.zdbjq.cn/Article/details/gugeaqzdy.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.hesvh.cn/Article/details/gqzrggplj.sHtML

esac
来源：http://m.share.hesvh.cn/Article/details/gnlrxtnzz.sHtML

[R12] for 遍历文件
来源：http://blog.hesvh.cn/Article/details/gmdfmxndq.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.hesvh.cn/Article/details/goebkeflw.sHtML

[R13] for 计数循环
来源：http://m.share.hesvh.cn/Article/details/gazgetgjb.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.fehbvm.com/Article/details/gdmbgpdhe.sHtML

[R14] C 风格 for
来源：http://mobile.hesvh.cn/Article/details/gpsijmkwi.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://baike.hesvh.cn/Article/details/gjfmbzwwc.sHtML

[R15] while 逐行读文件
来源：http://read.share.hesvh.cn/Article/details/gaswfkniw.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.fehbvm.com/Article/details/gxitfylru.sHtML

[R16] until 等待条件
来源：http://wap.zdbjq.cn/Article/details/geqwhluso.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.fehbvm.com/Article/details/gwdhpsboz.sHtML

[R17] 数组定义与取值
来源：http://baike.hesvh.cn/Article/details/guiukrify.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.zdbjq.cn/Article/details/gtbblhxdi.sHtML

[R18] 遍历数组
来源：http://m.share.zdbjq.cn/Article/details/gxbjuzcgu.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.hesvh.cn/Article/details/ggdygudkq.sHtML

[R19] 数组长度
来源：http://blog.zdbjq.cn/Article/details/gpzendpvo.sHtML

echo "${#arr[@]}"
来源：http://read.share.zdbjq.cn/Article/details/gmzvbppgs.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.hesvh.cn/Article/details/gilncbdxl.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.zdbjq.cn/Article/details/gnabnrtlw.sHtML

[R21] 字符串长度
来源：http://www.share.hesvh.cn/Article/details/gejxjhunf.sHtML

echo "${#s}"
来源：http://www.share.zdbjq.cn/Article/details/gwjahaluf.sHtML

[R22] 截取子串
来源：http://www.m.share.fehbvm.com/Article/details/gltsqvinc.sHtML

echo "${s:0:5}"
来源：http://www.m.share.zdbjq.cn/Article/details/guldexjsl.sHtML

[R23] 字符串替换
来源：http://wap.zdbjq.cn/Article/details/ggsqrznfz.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.fehbvm.com/Article/details/gleyhkgju.sHtML

[R24] 大小写转换
来源：http://read.share.fehbvm.com/Article/details/ghhmsjfko.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.zdbjq.cn/Article/details/gqsadrook.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.zdbjq.cn/Article/details/grlkdiqiv.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.hesvh.cn/Article/details/geapmyvth.sHtML

[R26] 命令替换
来源：http://m.share.fehbvm.com/Article/details/giieplnhp.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.fehbvm.com/Article/details/gwynwahyt.sHtML

[R27] 算术展开
来源：http://read.share.fehbvm.com/Article/details/gzpvixdda.sHtML

echo $((1 + 2 * 3))
来源：http://wap.fehbvm.com/Article/details/gmcfcmset.sHtML

[R28] 浮点运算
来源：http://wap.hesvh.cn/Article/details/gfqkbhczi.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.zdbjq.cn/Article/details/gsaqtuxlx.sHtML

[R29] 定义函数
来源：http://m.share.fehbvm.com/Article/details/gncwrxnbr.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.fehbvm.com/Article/details/gseihbphk.sHtML

[R30] 函数返回状态码
来源：http://m.share.zdbjq.cn/Article/details/gfjiupxex.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.fehbvm.com/Article/details/gwqactlkt.sHtML

[R31] 局部变量
来源：http://blog.zdbjq.cn/Article/details/gvmeglwmg.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.fehbvm.com/Article/details/gvqgnldrq.sHtML

[R32] 参数个数校验
来源：http://www.m.share.hesvh.cn/Article/details/ggqigabng.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.fehbvm.com/Article/details/ggizkdmws.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.fehbvm.com/Article/details/gpjybbhxk.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.fehbvm.com/Article/details/gipfhnrfe.sHtML

[R34] 退出时清理
来源：http://m.share.fehbvm.com/Article/details/gfrcvuqxo.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.fehbvm.com/Article/details/gvemnkoui.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.hesvh.cn/Article/details/govpdcrfv.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.zdbjq.cn/Article/details/gzlzreklu.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.zdbjq.cn/Article/details/gjkzyofnm.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.fehbvm.com/Article/details/gqwuuhsxt.sHtML

[R37] 把输出赋给变量
来源：http://baike.zdbjq.cn/Article/details/gxeafrqnj.sHtML

files=$(ls -1)
来源：http://baike.fehbvm.com/Article/details/gkdssjydk.sHtML

[R38] 管道串联
来源：http://www.m.share.zdbjq.cn/Article/details/gwdttnuzf.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.zdbjq.cn/Article/details/gxvpwwefw.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.fehbvm.com/Article/details/gwlnxcmqe.sHtML

cmd > out.log 2>&1
来源：http://blog.hesvh.cn/Article/details/gbnvyuuju.sHtML

[R40] 追加写日志
来源：http://3g.fehbvm.com/Article/details/gwklsyscx.sHtML

echo "log" >> out.log
来源：http://baike.fehbvm.com/Article/details/givndcmzm.sHtML

[R41] 丢弃输出
来源：http://baike.zdbjq.cn/Article/details/gunusplkw.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.hesvh.cn/Article/details/gfuhtgacd.sHtML

[R42] 输入重定向
来源：http://mobile.hesvh.cn/Article/details/gxdknicgv.sHtML

wc -l < a.txt
来源：http://baike.zdbjq.cn/Article/details/gatwxqrhj.sHtML

[R43] 按名字查找文件
来源：http://wap.hesvh.cn/Article/details/gtdiimfjy.sHtML

find . -name "*.log" -type f
来源：http://wap.fehbvm.com/Article/details/gmtwpwcpn.sHtML

[R44] 按修改时间查找
来源：http://baike.fehbvm.com/Article/details/gqjtswukx.sHtML

find . -mtime -7 -type f
来源：http://read.share.zdbjq.cn/Article/details/gprwpelwx.sHtML

[R45] 批量删除
来源：http://baike.zdbjq.cn/Article/details/glxojpyhq.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.fehbvm.com/Article/details/gsykbzlih.sHtML

[R46] 递归替换文件内容
来源：http://3g.zdbjq.cn/Article/details/gsmyfspoj.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.hesvh.cn/Article/details/gwgczssow.sHtML

[R47] sed 单行替换
来源：http://blog.zdbjq.cn/Article/details/gxkfcugbt.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.hesvh.cn/Article/details/gxmexvoqy.sHtML

[R48] awk 取指定列
来源：http://baike.hesvh.cn/Article/details/gwlzxtwhd.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.hesvh.cn/Article/details/gthqwokqw.sHtML

[R49] awk 带条件
来源：http://m.share.hesvh.cn/Article/details/ghdavmaly.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.zdbjq.cn/Article/details/gemvbyrsj.sHtML

[R50] awk 求和
来源：http://baike.hesvh.cn/Article/details/gtcvyflai.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.fehbvm.com/Article/details/gbabkxucq.sHtML

[R51] 排序去重取前几
来源：http://m.share.zdbjq.cn/Article/details/grobuilvo.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.hesvh.cn/Article/details/geajibrks.sHtML

[R52] 统计行数
来源：http://blog.hesvh.cn/Article/details/gdvngphpi.sHtML

wc -l a.txt
来源：http://mobile.zdbjq.cn/Article/details/gjeeahpdo.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.zdbjq.cn/Article/details/gnrcgipwv.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.zdbjq.cn/Article/details/gjxribyjl.sHtML

[R54] 比较两个文件
来源：http://wap.hesvh.cn/Article/details/gnynryyzm.sHtML

diff a.txt b.txt
来源：http://3g.fehbvm.com/Article/details/ggdbfzfxt.sHtML

[R55] 压缩与解压
来源：http://www.m.share.hesvh.cn/Article/details/goxkxjbfp.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.fehbvm.com/Article/details/gzhklelnj.sHtML

[R56] 远程拷贝
来源：http://www.m.share.zdbjq.cn/Article/details/gacsdhqrd.sHtML

scp file user@host:/path/
来源：http://wap.zdbjq.cn/Article/details/gwhcqxoxe.sHtML

[R57] 远程执行命令
来源：http://read.share.fehbvm.com/Article/details/gqeyaqyuy.sHtML

ssh user@host 'uptime'
来源：http://baike.hesvh.cn/Article/details/gqgnipgfa.sHtML

[R58] 下载文件
来源：http://www.blog.fehbvm.com/Article/details/gwjvwdhek.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.zdbjq.cn/Article/details/gatoawlph.sHtML

[R59] 发 POST JSON
来源：http://www.share.fehbvm.com/Article/details/gocfidknj.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.hesvh.cn/Article/details/gwgrephpq.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.hesvh.cn/Article/details/gmcscpqli.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.zdbjq.cn/Article/details/gkvbcjxhq.sHtML

[R61] 磁盘占用
来源：http://read.share.hesvh.cn/Article/details/gpotbswjk.sHtML

df -h;  du -sh *
来源：http://www.share.zdbjq.cn/Article/details/gfrelxffe.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.hesvh.cn/Article/details/gutgegfra.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.zdbjq.cn/Article/details/gbcaljyxw.sHtML

[R63] 内存与进程
来源：http://blog.fehbvm.com/Article/details/gjqcmmtyy.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.hesvh.cn/Article/details/ggklixzut.sHtML

[R64] 结束进程
来源：http://read.share.hesvh.cn/Article/details/gidrcpxta.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.zdbjq.cn/Article/details/gxifcjdzo.sHtML

[R65] 查看端口占用
来源：http://3g.fehbvm.com/Article/details/gpfibdgfi.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.zdbjq.cn/Article/details/gyzupayrn.sHtML

[R66] 定时任务
来源：http://wap.fehbvm.com/Article/details/gplnqvrfv.sHtML

crontab -e;  crontab -l
来源：http://wap.fehbvm.com/Article/details/gndhmprcf.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.zdbjq.cn/Article/details/gsmbcpfnb.sHtML

openssl rand -hex 16
来源：http://www.share.fehbvm.com/Article/details/gtgomhphi.sHtML

[R68] 计算文件校验值
来源：http://blog.fehbvm.com/Article/details/ggngbicic.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.hesvh.cn/Article/details/ghtrmugyw.sHtML

[R69] 生成随机密码
来源：http://mobile.fehbvm.com/Article/details/grlckiirk.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.hesvh.cn/Article/details/grnowkuxo.sHtML

[R70] 时间戳与互转
来源：http://m.share.zdbjq.cn/Article/details/gdgfvdnff.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.zdbjq.cn/Article/details/gtbykxfbx.sHtML

[R71] 日期格式化
来源：http://wap.hesvh.cn/Article/details/gpzpmxykn.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.zdbjq.cn/Article/details/gnijtoyyf.sHtML

[R72] 等待端口就绪
来源：http://read.share.hesvh.cn/Article/details/gnnzgytbr.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.hesvh.cn/Article/details/gliuhxsge.sHtML

[R73] 分割大日志
来源：http://www.blog.fehbvm.com/Article/details/gduhlovoy.sHtML

split -l 1000 big.log part_
来源：http://3g.hesvh.cn/Article/details/gnkwdqvgc.sHtML

[R74] 批量重命名
来源：http://www.share.fehbvm.com/Article/details/gwvpxtbqn.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.zdbjq.cn/Article/details/gsmrsmfjo.sHtML

[R75] 导出环境变量
来源：http://baike.zdbjq.cn/Article/details/gqxncgxfq.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.zdbjq.cn/Article/details/gfygqelgh.sHtML

[R76] 使用临时文件
来源：http://mobile.fehbvm.com/Article/details/gqefqzcua.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.zdbjq.cn/Article/details/gmkckwwbh.sHtML

[R77] 读取用户输入
来源：http://3g.fehbvm.com/Article/details/ghowmhqgq.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.hesvh.cn/Article/details/grdoanuxg.sHtML

[R78] 交互式菜单
来源：http://www.blog.fehbvm.com/Article/details/gwhdiqpmh.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.hesvh.cn/Article/details/gkmtkwpfz.sHtML

[R79] 解析命令行选项
来源：http://www.blog.zdbjq.cn/Article/details/gddkxhdtz.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.fehbvm.com/Article/details/gyylblzpg.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.fehbvm.com/Article/details/ghidvolla.sHtML

time ./run.sh
来源：http://baike.hesvh.cn/Article/details/gaeukgybm.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/grkkoimhp.sHtML

S. C / C++ 专题
来源：http://mobile.hesvh.cn/Article/details/gfalrbjbc.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gdvrapawk.sHtML

[S01] C：Hello World
来源：http://www.share.hesvh.cn/Article/details/gatffcpkh.sHtML

#include <stdio.h>
来源：http://m.share.hesvh.cn/Article/details/gkcgoenhe.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.hesvh.cn/Article/details/gyeaqfdyn.sHtML

[S02] C：变量与格式化输出
来源：http://wap.hesvh.cn/Article/details/gksykkpoj.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.zdbjq.cn/Article/details/gbwngrdaa.sHtML

[S03] C：读入整数
来源：http://blog.hesvh.cn/Article/details/gstfvfyon.sHtML

int x; scanf("%d", &x);
来源：http://m.share.hesvh.cn/Article/details/gebvniyvx.sHtML

[S04] C：字符串复制
来源：http://wap.hesvh.cn/Article/details/goqybodna.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.fehbvm.com/Article/details/gmagbkrgb.sHtML

[S05] C：字符串长度
来源：http://wap.fehbvm.com/Article/details/gmbsztjmm.sHtML

strlen(s)
来源：http://www.m.share.fehbvm.com/Article/details/guxeqjqtq.sHtML

[S06] C：字符串比较
来源：http://www.m.share.zdbjq.cn/Article/details/ghjngmoqk.sHtML

strcmp(a, b) == 0
来源：http://mobile.hesvh.cn/Article/details/gfcgbrlhw.sHtML

[S07] C：数组遍历求和
来源：http://blog.hesvh.cn/Article/details/gwwseppoy.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.hesvh.cn/Article/details/gdstmrdmf.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.fehbvm.com/Article/details/geuxsccte.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.hesvh.cn/Article/details/gmocabute.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.fehbvm.com/Article/details/glxtqsgmv.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.hesvh.cn/Article/details/gdrikqauc.sHtML

[S10] C：指针与解引用
来源：http://wap.hesvh.cn/Article/details/gnokqmpio.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.zdbjq.cn/Article/details/gkyktpkso.sHtML

[S11] C：逐行读文件
来源：http://www.blog.hesvh.cn/Article/details/gvuoawwbs.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.zdbjq.cn/Article/details/giqoiaujl.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.fehbvm.com/Article/details/gfmxkcajf.sHtML

fclose(f);
来源：http://www.m.share.hesvh.cn/Article/details/gbhtmoijh.sHtML

[S12] C：写文件
来源：http://www.m.share.fehbvm.com/Article/details/gbzcbyoxq.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.fehbvm.com/Article/details/gjqsocvzr.sHtML

[S13] C：宏定义
来源：http://3g.zdbjq.cn/Article/details/gplxaiady.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.fehbvm.com/Article/details/gvbshlwtl.sHtML

[S14] C：枚举
来源：http://www.blog.zdbjq.cn/Article/details/gngmxdvrj.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.fehbvm.com/Article/details/gpyyxvvhx.sHtML

[S15] C：类型转换
来源：http://read.share.hesvh.cn/Article/details/gzykjieyq.sHtML

(double) a / b
来源：http://www.blog.fehbvm.com/Article/details/gkhwumolf.sHtML

[S16] C：位操作置位
来源：http://www.share.fehbvm.com/Article/details/gnikdnqrv.sHtML

x |= (1 << 3);
来源：http://m.share.fehbvm.com/Article/details/gwwwqngah.sHtML

[S17] C：安全拼接字符串
来源：http://baike.zdbjq.cn/Article/details/gajwwseuv.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.zdbjq.cn/Article/details/gjxkrxatk.sHtML

[S18] C：命令行参数
来源：http://read.share.hesvh.cn/Article/details/gkfayyflj.sHtML

int main(int argc, char **argv)
来源：http://wap.zdbjq.cn/Article/details/godvwauta.sHtML

[S19] C：快速排序
来源：http://mobile.fehbvm.com/Article/details/gdftkipza.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.hesvh.cn/Article/details/grodnafbb.sHtML

[S20] C：二分查找
来源：http://www.m.share.hesvh.cn/Article/details/gkyltpdlo.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.fehbvm.com/Article/details/gjuajroli.sHtML

[S21] C：字符类别判断
来源：http://read.share.fehbvm.com/Article/details/gkbspdgjo.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.fehbvm.com/Article/details/gwythxzzn.sHtML

[S22] C：字符串转数字
来源：http://read.share.fehbvm.com/Article/details/geednjgdh.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.hesvh.cn/Article/details/gqzivreyr.sHtML

[S23] C：随机数
来源：http://wap.zdbjq.cn/Article/details/gbedpbtok.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.zdbjq.cn/Article/details/gozbwgmhf.sHtML

[S24] C：获取本地时间
来源：http://www.blog.fehbvm.com/Article/details/gpoxmvlzf.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.fehbvm.com/Article/details/gprcqhtpy.sHtML

[S25] C：内存拷贝
来源：http://baike.hesvh.cn/Article/details/gothrajdo.sHtML

memcpy(dst, src, n);
来源：http://www.blog.hesvh.cn/Article/details/goyxockgm.sHtML

[S26] C：内存清零
来源：http://www.blog.fehbvm.com/Article/details/gnbucjgdj.sHtML

memset(a, 0, sizeof a);
来源：http://blog.zdbjq.cn/Article/details/gookfyskl.sHtML

[S27] C：定义常量
来源：http://www.share.fehbvm.com/Article/details/gihqiwwij.sHtML

const double PI = 3.14159;
来源：http://www.blog.zdbjq.cn/Article/details/grutvzlim.sHtML

[S28] C：静态变量
来源：http://www.share.fehbvm.com/Article/details/gcdgutcrt.sHtML

static int counter = 0;
来源：http://www.m.share.zdbjq.cn/Article/details/gazaqpofv.sHtML

[S29] C：变参函数
来源：http://baike.hesvh.cn/Article/details/guihihytm.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.fehbvm.com/Article/details/gymlrskyz.sHtML

[S30] C：头文件保护
来源：http://mobile.fehbvm.com/Article/details/gvtstturs.sHtML

#ifndef X_H
来源：http://baike.zdbjq.cn/Article/details/gjhtnppuz.sHtML

#define X_H
来源：http://wap.fehbvm.com/Article/details/gemxihnwc.sHtML

#endif
来源：http://baike.hesvh.cn/Article/details/gjqsbhcpq.sHtML

[S31] C++：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gsqvxwhtk.sHtML

#include <iostream>
来源：http://mobile.zdbjq.cn/Article/details/gvwihgcve.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.hesvh.cn/Article/details/gacaorhdq.sHtML

[S32] C++：字符串
来源：http://mobile.hesvh.cn/Article/details/gmoiqwzuy.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.zdbjq.cn/Article/details/gweknrlnr.sHtML

[S33] C++：vector 增删
来源：http://www.blog.hesvh.cn/Article/details/grecvgbbp.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.hesvh.cn/Article/details/gyfnligyj.sHtML

[S34] C++：遍历 vector
来源：http://read.share.fehbvm.com/Article/details/gdekfwivh.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.fehbvm.com/Article/details/getlbsecl.sHtML

[S35] C++：map
来源：http://www.share.hesvh.cn/Article/details/gwbyvlelb.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.hesvh.cn/Article/details/godfrktbd.sHtML

[S36] C++：unordered_map
来源：http://blog.fehbvm.com/Article/details/gbunzjrkt.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gsvyiffsn.sHtML

[S37] C++：set
来源：http://3g.hesvh.cn/Article/details/gmjmoluqc.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.fehbvm.com/Article/details/gztgskuae.sHtML

[S38] C++：排序
来源：http://3g.fehbvm.com/Article/details/gsghwxslh.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.hesvh.cn/Article/details/gqnqolbzb.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.zdbjq.cn/Article/details/gqffsqynp.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.hesvh.cn/Article/details/glzlryxap.sHtML

[S40] C++：查找元素
来源：http://mobile.fehbvm.com/Article/details/glaaqnsmh.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.hesvh.cn/Article/details/gcnzsexvm.sHtML

[S41] C++：类与构造函数
来源：http://3g.hesvh.cn/Article/details/gqyxppxlu.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.hesvh.cn/Article/details/gjpddwbrp.sHtML

[S42] C++：继承与虚函数
来源：http://blog.zdbjq.cn/Article/details/ghicigmpl.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.zdbjq.cn/Article/details/gcncnbsgc.sHtML

[S43] C++：智能指针
来源：http://mobile.hesvh.cn/Article/details/gwdaxzuor.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.fehbvm.com/Article/details/gyyzmofbz.sHtML

[S44] C++：引用传参
来源：http://read.share.zdbjq.cn/Article/details/glcbfdjrv.sHtML

void inc(int &x) { ++x; }
来源：http://3g.hesvh.cn/Article/details/gfngficyi.sHtML

[S45] C++：lambda
来源：http://www.m.share.fehbvm.com/Article/details/gtcivcxlk.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.zdbjq.cn/Article/details/gkdwmpkjf.sHtML

[S46] C++：函数模板
来源：http://read.share.zdbjq.cn/Article/details/gvmccsdrp.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.hesvh.cn/Article/details/gnzsqazrj.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.hesvh.cn/Article/details/gbegnrcru.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.fehbvm.com/Article/details/gdejrorpg.sHtML

[S48] C++：逐行读文件
来源：http://baike.hesvh.cn/Article/details/gmrxqiqxp.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.fehbvm.com/Article/details/gkufssvev.sHtML

while (std::getline(in, line)) { }
来源：http://baike.hesvh.cn/Article/details/gfeenjxbm.sHtML

[S49] C++：写文件
来源：http://www.share.fehbvm.com/Article/details/gszxxffay.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.hesvh.cn/Article/details/gydybqxat.sHtML

[S50] C++：格式化数字
来源：http://www.share.fehbvm.com/Article/details/gsixnvvcm.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.hesvh.cn/Article/details/gopcfyyqb.sHtML

[S51] C++：显式类型转换
来源：http://read.share.hesvh.cn/Article/details/gwcnegwfy.sHtML

static_cast<double>(a) / b
来源：http://blog.fehbvm.com/Article/details/gdxuhqtcy.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.zdbjq.cn/Article/details/gfzzaqani.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.zdbjq.cn/Article/details/gxxiejnhn.sHtML

[S53] C++：移动语义
来源：http://3g.fehbvm.com/Article/details/geibjbyjr.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.fehbvm.com/Article/details/gzyqzzxod.sHtML

[S54] C++：异常处理
来源：http://www.m.share.zdbjq.cn/Article/details/glickkpwq.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.zdbjq.cn/Article/details/glxlsgcel.sHtML

[S55] C++：结构化绑定
来源：http://baike.fehbvm.com/Article/details/gojvdnybg.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.hesvh.cn/Article/details/gsklgzrca.sHtML

[S56] C++：optional
来源：http://wap.hesvh.cn/Article/details/gdyphtqxj.sHtML


<!-- 参考信息 -->