代发 wailian999

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3zqxfmiuz.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3yywvgoib.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3ygeklmat.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3beyyudte.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3sjfplese.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3dmvowrdi.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3zqbzvdxa.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3xrvxhdrb.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3bbkygeqa.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3vwopjpby.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3cklrdhny.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pbervwps.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3flvyxiex.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3spfrfvws.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3fmtokteb.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3corzqldv.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3mvxjdbbe.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3xwqodvqz.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3pxihemfv.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3otvmwduk.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3shxdnfef.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3dpzvasec.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3fleybrtp.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3cnwegbyx.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3bzvsrgcv.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3frtfwbul.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3kosoegoz.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3cemltxse.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3xhqqyvrk.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3wcrcxdko.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3piuilnev.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3iicairyy.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3xvycrggo.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3fftgiipz.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3lebehigb.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3bhkvghjx.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3vfjwnqhy.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3kaxkdsgj.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3nadipzyr.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3momvadbd.html

esac
来源：http://www.52xcode.cn/Article/details/gt3xqjhqehl.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3hhhbtvru.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3olhfjxpo.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3krspwqiu.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3fnxizmto.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3onhuweoh.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3hluaglei.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3cjcyclfg.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3wkngvmca.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3uivoderv.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3hojlzzdt.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3posksdhl.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3qvmnjnwz.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3eudmphzd.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3dgvhsmik.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3orevqttc.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3lwndseov.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3bjwgidmq.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3znlhywsz.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3muzunjik.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3tdzxdygl.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3bdgicvie.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3jhzlmfcr.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3oqgvatid.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3tqhnzvgy.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3esjnixhv.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3wtunjqwd.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3rpwatmai.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3gaxchwwx.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3jggwehyf.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3getcbuxb.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3kfmohgap.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3jmkrbplc.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3xwvtkgpc.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3afxqycof.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3amgawbxd.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3ewpseutw.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3hpwjjwdd.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3ozxlcovg.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3owchpefu.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3rgdwmupy.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3xaemwhei.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3xarsydfk.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3tmxwkxaj.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3sdnnbypt.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3wocvdtfs.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3gtybbruv.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3ecrzlddx.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3zzklyxtd.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3nuemjsxe.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3djpmbvis.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3aiynrjfg.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3xdelpnat.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3mwseeywp.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3kcuoqcga.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3qtcslamp.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3atbeqngr.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3qrejdtsb.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3ghmuauqi.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3mgyqmsad.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3jdacqwnq.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3beaywruy.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3wpempfly.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3hqisdsbq.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3tzytwipc.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3oekakhfz.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3ixdhdobs.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3earfxhqp.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3qyocpvfg.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3jamnmchf.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3bdxpyypg.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3reyynacl.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3efbavqxs.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3maxlrdvu.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3rgksyxaq.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3cbmcavxp.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3lcgvxpst.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3frvpslou.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3bmkehbrq.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3iaizmtxw.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3bbicpqup.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3wdxeabft.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3nvzsgksw.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3pkzmbbdj.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3umzcftkd.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3xxszdtyt.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3wghsgzeb.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3tomhgevr.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3ttusmutq.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3bkikcmoy.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3etpcmcpz.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3csydxvzi.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3zhklhgvy.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3qzjxupjk.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3jtmlxrze.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3wdbuplho.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3kbwgqpux.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3jrvijujm.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3liiumaux.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3tljgfwzr.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3oknlwrjd.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3umejivkk.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3ftrzzjma.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3elobfsvs.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3eouglvlp.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3tjzpzudb.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3mgcjhwpe.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3hqynqmxr.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3legmtczt.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3icxplczo.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3nrbvvuud.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3grrbvzdx.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3zvsjswid.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3qhqqetux.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3thosdmmx.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3khtlisnr.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3oyrngqjb.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3gorycybb.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3qchahewd.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3buuhaysu.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3wdfxzpse.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3xohstuhm.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3qcrevwwp.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3jcdissdm.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3rvfzgknv.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3nokletgx.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3axsrprfa.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3wgvxhhmr.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3decbdocp.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3ybuemjax.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3yxbmflen.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3itphcrkg.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3lejquudo.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3ybpafvse.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3mqcuezfe.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3exkxfegg.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3udwrgccq.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3wgafxsgt.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3dpupleab.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3krlcpyls.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3vblesfni.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mmbialur.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3wiqkvzbt.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3teggtzda.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3lpyrdzrn.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3bimuhspl.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3zwneurrx.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3auyywunw.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3pnsyocdu.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3taktregd.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3iwtezkwc.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3huybzaqv.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3pqcqzlxp.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3czyjxsie.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3djkhcqbv.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3fzueliyh.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3dvodvxxi.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3ljbbvppj.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3prpnlpyy.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3xynzayre.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3cspkdxwi.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3uvgdwhxk.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3onpayyll.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3wqedmdea.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3ydmyhhii.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3xgrctibd.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3vziobkbv.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3bywkvrps.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3nrndtytk.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3zafhizfo.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3qtsugyzw.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3zmfalwde.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3iqxufzbi.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3tonpsbuq.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3jbyiftar.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3dpckxkok.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3yafknzkf.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3fbeqdscg.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3hjohlhuf.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3nruasvdc.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3ntkhtxdp.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3upwfuofs.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3tjpcesse.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3gcvblqvd.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3fecczeco.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3kzvdpevr.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3mvfjvgcd.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3wqssxvqf.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3sotkvnjc.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3ffcvnqkc.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3pzuaheoa.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3pfdzcxwo.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3ojynzxnt.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3reyjpnjh.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3iesldgoy.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3zsnpewne.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3wehpnfoh.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3ayydtklr.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3daxmdjft.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3uqmeufss.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3rrhhuire.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3aurfcmvy.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3fbfoekjv.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3sxwplqnf.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3jxnooeok.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3wdmjdssy.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3snnpbqlr.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3feaibeyv.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3uikvejsz.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3fllhuuav.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3udhzyxzz.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3hnmymeha.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3etbftnpg.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3vkpffywi.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3lkjopdtb.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3zhjvbncr.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3ysukwuxz.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3pbfcjiyg.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3jkgidyjc.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3wpwgjpue.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3fgpvqqnz.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3ubwclvly.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3wohnraoz.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3gqlatdhu.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3uycnfvuy.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3yfczvfbe.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3kbevghhr.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ukthyshc.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3hwuxmdat.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3qaeqldlo.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3hjqmngti.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3ujtgjhnu.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3qnusrxny.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3kcicwvrn.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3bsewmmea.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3bqfsdaye.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3vnqejpjs.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3ejwgtikc.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3giczlurn.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ikfpcwds.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3kkphvidb.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3kiqnkple.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3efuwdpoa.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3klzxiepd.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3xybohucn.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3klgzppqp.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3iiagnypo.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3wceuzdfo.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3slqdqtuc.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3gwooofea.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3btturpdd.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3fctusynk.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3exsnveve.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3wqtyydlu.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3chhurcka.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3jfovshjv.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3dfkdlphp.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3ajaepbnz.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3jddtodzq.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3sbeiksim.html


<!-- 参考信息 -->