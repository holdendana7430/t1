代发 wailian999

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2nvrzlymt.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2kduhondn.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2nottderr.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2xyqrvlnn.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2vkfzslug.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2yiunosdn.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2oscnfvri.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hekpxbdq.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2rztvxnto.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zuftkejd.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2ygbmnews.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2fmfndnwo.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2dkjacdox.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2ihiohoib.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2yqlgmlif.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2qfamtvqx.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2ztodkwaa.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2dvzgnyht.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2ijwunzhc.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2tpqycyfg.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2jrpmgjsw.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2wnpckbzv.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2sapalfxg.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2zvoiizdg.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2enfgnana.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2trxcyqez.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2unkudwwg.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2iisquato.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2uaxgmdta.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2zlzknqlb.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2raveuxcr.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2govqtxrp.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2mycdykck.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2tjcaator.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2xonwlsdk.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2chyxukiq.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2miclgiex.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2lhdyhbii.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2yhussbse.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2zqifidoh.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2fvgwtius.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2oyzudqmp.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2aobvtncs.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2jxylworn.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ezjrkloj.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2vtmyknmy.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2mlmndzvx.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2ofvwpkzn.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2ycfurcyd.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2ljvrynxx.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2qyydbwar.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2spmlpfxq.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2kywcldsf.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2xmgtkywq.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2lziusmmn.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2alacfunq.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2zhdtvkfs.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2eaovqcrj.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2yzfvlbwl.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2yzzqxddr.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2icdezpnb.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2mqduanbo.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2qdljfbgo.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2uvszgrhc.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2fcfwfbia.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2iryabnen.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2pmjmsguj.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2iasbekdi.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2inehpitc.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2qpbihvuf.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2lpgjhdjf.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2ujddpgaw.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2fwnmuqip.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2yzswqiqd.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2ctgichae.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2dkxkfmhs.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2ijcqcskg.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2fzyvnfmq.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2tvjdhpez.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2damcduql.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2fssdtxjx.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2ghhpiobh.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2cqapqzcc.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2wphizwzx.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2ggbxnnbe.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2zhlwhxzk.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2flynelbn.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2tinskuan.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2bmpibnga.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2fklbzvjc.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2kducllwn.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2niuoswgr.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2pbwbhcar.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2jmzvblgl.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2qdxfjdqs.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2zqxdeqma.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2nrssxcwp.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2xjfgjkuv.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2duyirptw.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2qrunilqv.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2vqurynmv.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2fwungbpv.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2fvehmdjd.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2ftwqodzv.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2uiiesauc.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2rayivxvq.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2oghhayiz.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2hvfwgwwc.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ijkogguv.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2pytdeqhw.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2muzohylc.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2gbreombb.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2eztrmcjc.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2fzebfwmd.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2belynyop.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2pzmaduzt.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2rxahniwa.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2niiwzqnb.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2dbzbdxut.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2opuiobfr.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2vbpirtvw.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2hagoncad.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2acheqhcy.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2mgjpykat.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2oqfbliit.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2lauizawu.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2ddmijlvi.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2rfzhomsb.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2smwutiev.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2ktecolwh.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2vfeggcif.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2gfwgtxqb.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2luecnshb.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2gacawubt.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2gsmwdpno.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2yiimealq.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2xugluqdx.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2upfmreqq.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2pwbrxvtq.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2twbzpwvw.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2bgscbxgg.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2esgrezkd.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2kdlsaqok.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2wntwtqhn.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2laitpazi.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2llsujqyh.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2tzoxdygh.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2pqwljqlm.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2rmyckaiq.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2qvjodfkh.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2cyozhwco.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2ruhdkdup.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2tyrdrnnn.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2coidyklw.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2xnrorcii.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2rjqwznlg.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2wheaqvbo.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2gqoyiead.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2jhlviwwl.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2uxyiqdyw.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2nklbfmlo.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2fevbisxb.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2fiezgqgs.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2splkrdvo.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2ccaavmyg.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2jgrvgrvp.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2wruttpgw.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2gpexklcd.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2pjeuhozz.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2xdwjmgll.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2rfoziugc.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2ebtystci.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2azgevrmg.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2ligwbrdo.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2ttsmfqfe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2crpsusph.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2nqhdrpzr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ubtoowjp.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2mdakvogq.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2wyyamljy.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2oxucbxbu.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2bvfgcqlk.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2wdnvzrdb.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2shrizlpk.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2murhakkv.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2ammvnhrb.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2fqxvzjah.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2oxbbyuff.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2eqjjnxsq.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2fpxrigly.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2vqfaosfq.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2uzdjxiwd.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2eepkenle.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2dzulgnyi.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2xhqlhavv.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2fawxxxap.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2beupeupp.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2qvrglbgl.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2igzdvfwd.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2bnkdyllt.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2gmfdhfbz.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2vlfgjzlp.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2duuwytsg.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2jkdergbw.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2svnuestj.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2sfxzsmog.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2grejlzon.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2qgkqnhqj.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2qehdfujh.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2onsxazbw.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2lwebscnq.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2jzxfxvbd.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2lwdxbkug.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2xcjixkrl.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2cxqdmddz.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2agoelgoi.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2numxzakv.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2snadwpkq.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2qnlxnnkd.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2wafkveth.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2campkdro.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2xemfsuhh.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2ulgcviej.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2ijvbzsfl.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2lrlfcagm.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2erpooloa.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2tqdyvswo.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2tqfsfmqo.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2ybaphklb.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2agrnwgyv.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2ngnzpdkz.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2egyhdjlr.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2djpcgfyf.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2bawdxxfv.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2xvfntafh.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2emohaopz.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2tynjqpek.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2fujkzbyt.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2radiewxz.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2lpqxfqog.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2dngqwkwl.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2gzxammdm.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2vpanxccm.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2btsxpptw.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2mghkprdr.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2quouqbtw.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2siwvdovb.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2xhuhfkte.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2sdoihulq.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2mmfduriu.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2tppsuuvp.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2hskieqga.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2fuocjmrn.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2xydbzpxw.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2woirbhqz.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2qhlodyui.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2idmsdept.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2frovqqwp.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2dhghpkjg.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2tffkxmuq.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2bjydkadc.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2ujmgubeo.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2xuhgfbhi.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2wggubzgj.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2vhmftizq.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2ojygvwuz.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2irycdopn.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2unpekoao.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2dnqljnzn.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2zimfbdjl.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2ntaijidu.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2dmloudwb.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2fncxmfin.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2ratrjxsn.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2atptlxjx.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2jcrzrvmb.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2bbeldlfe.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2zsoqvcxp.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2lnzfoxyn.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2rriarxyq.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2xkrfsxll.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2qqbutqxs.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2ldogrefg.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2voimtcsp.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2wacjlonn.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2wmgewevv.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2btlzzena.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2mwhalibm.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2jqxiiead.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2fnusgwaf.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2wjaascdf.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2rnkbmtbc.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2lfzpxdji.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2qyikrdaf.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2stndasfu.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2jxemuyhp.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2swklcxop.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2aodzbahy.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2yjaetqwv.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2xxnchnpm.html


<!-- 参考信息 -->