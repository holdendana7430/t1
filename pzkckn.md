代发 wailian999

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2ytgkyvom.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2mbnbenpo.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2pzwywlzq.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2lsskugum.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2veoynwsz.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2npofgsjd.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2zxntqaqw.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2glovtifs.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2wjogefph.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2fmkomeaa.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2frsnhpyl.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2jigyksfn.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2ukaecewg.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2nkegskng.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2xzkuzwva.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dsoithvw.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2qvbgxomg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ksxyrdci.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2dttnycai.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2cnrotwre.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2ndyuqepp.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2ojjbnwgr.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2qqcccdoz.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2rgktszxa.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2umhytfnj.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2xvqkzwvp.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2snzkwjqb.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2jutnbflg.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2vvovhqvl.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2dtvuzefb.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2xxaikngz.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2blrkfcky.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2wsutwubt.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2nbvlaguy.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2axeeytox.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2ongmbrvd.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2biizyhnw.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2kctiixzm.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2kiqyunap.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2rclqijzn.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2ymugfups.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2jsxapkqg.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2sxtlndzt.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2iocokfcg.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2rourzzxm.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2sejsxetp.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2egsruagu.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2isamcqgz.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2hcciujsa.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2rlsazgeo.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2mizminko.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2ssttyoep.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2jfjuqtxo.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2iqqnxcih.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2wygabyrs.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2bozfnhxo.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2svvadnut.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2xbocbzmw.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2qthuvbee.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2ppytxcav.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2hdwjppuy.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2aivjygnr.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2hqtptfhh.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2sfvvbttz.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2rodvbxxw.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2pkslyhfe.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2oaqghicm.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2cupqtvvi.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2ofpfeiev.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2xmkqgend.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2nvoiahdl.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2trssgvyk.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2gqpxqidu.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2kbkhpuoy.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2yzikpeiq.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2xagkdfnc.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2cackunau.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2nhjobmhi.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2wgqnnwxi.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2halznkae.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2bupfecmp.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2bhfciylq.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2odvxkuxm.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2loccnnwk.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2djbdokfn.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2andqipfk.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2xeetqdrd.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2bhfivdip.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2iqjkcyyq.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2yzfuusdv.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2ehhjlbex.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2klctxwpu.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2cmsmhmcp.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2yiwsswof.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2kmrbqtor.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2kugjruzq.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2gkjqmbfs.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2msvdrxoi.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2svxnmwhm.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2vadtewlo.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2ypxxuqck.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2argebsqk.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2euoyqzaq.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2engrkxdf.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2xntyvwnb.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2gbaklram.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2anffivav.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2fuczfobw.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2iwccolrz.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2iejrcczp.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2rqeeftrk.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2mtrziryy.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2ppofzgnu.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2arshssvm.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2trlahsrl.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2ztakvrot.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2bkoupqww.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2unhgmxnk.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2qghwjbvg.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2xyivjnel.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2qmnpbzgj.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2hytljvlt.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2jtomfksx.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2cyhmizjv.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2wdvlruiw.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2uyxrphgk.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2bcmeoosr.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2oirjjgyp.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2qdpwmdvp.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2loisimvg.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2ndwsytmt.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2nrpbphyl.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2vxzsucvk.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2npxudjwa.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2gbloxejl.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2hesovlvn.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2ngygijmg.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2gozaqcqi.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2wtujkcvx.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2qvchmkod.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2kajyfvzx.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2jijulnqa.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2eeyeypra.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2aqwjuapi.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2beqtrmiz.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2udnqydie.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2hxhtmoee.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2pqdrrslf.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2dosxosov.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2xzyjlswd.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2nydacjmg.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2ydkgnnfe.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2snnxntfy.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2lgceobsx.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2lorttkya.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2achweuud.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2bcbmtkys.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2ojjhrdxs.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2atolwawi.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2udhupzdv.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2shtjqcqa.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2jjrsmchj.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2ysinmbob.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2qvbmizqs.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2casauxwq.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2icsavwmw.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2vubjsoni.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2tprzyfvr.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2zjhcdhrl.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2nzntdtxp.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2cmngbbvs.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2aiqkjabn.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2vpqygdpj.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2hqfeubgo.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2gmbtjbdb.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2wagtaobj.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2uqhcbmbj.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2ajagjumz.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2ljhrdntn.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2pmlyzgzd.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2wbwqyshl.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2lvltltfj.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2rxomjsnb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2htgumflp.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2nzddtxgg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2odkpqgsh.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2xqngukmx.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2yzkfpvdv.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2orfbrgml.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2qmmajvao.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2rutlerwk.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2wfugoynr.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2vzeystgk.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2yjmnllxh.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2sxwutlsb.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2lmeihszk.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2oidmvufb.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2poyumceg.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2wmpewnry.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2kwvmbzdj.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2eibgderu.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2nbqetfja.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2acskvbhn.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2snmpbxqv.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2rtpdnqrt.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2rywcedke.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2ryrumpon.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2kteqeqjl.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2fpjrynoc.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2xdzssovn.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2llahgckh.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2vemhrmza.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2objuidrn.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2uxtrlozb.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2fljxtvji.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2lvypvmre.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2dwucetnf.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2qwjumyod.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2qckyesix.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2obiqtceb.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2xmaaoypl.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2fvdzrgbz.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2amedcboc.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2qaoklmhr.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2pdsrxcrg.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2afttcsde.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2xohgfhbn.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2njmouhco.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2cncathfm.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2dkdsuqtq.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2vbebzdiv.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2teemhfgv.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2cfblixwy.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2jwfcqqbj.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2zwbdaiep.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2zbppwapn.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2wkffaaci.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2recapned.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2eauxgihq.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2rzpdrzcu.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2uainhioz.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2zcuycxgf.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2scbcivgj.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2wharhcer.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2cdpkvsta.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2anrcisuq.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2ikltijjl.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2chlldwwk.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2gmomzzyh.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2nrhkgjjv.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2bfockbjr.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ecusyzry.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2rfvctsif.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2wlelifnv.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2rfgthvdp.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2jjctrjis.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2yhywmtog.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2zszmntmm.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2pxfdgvfy.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2tdwomnfq.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2phfrobvw.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2wjavpasl.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2ylmfjyre.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2upukwgfo.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2havomniy.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2hlpebciw.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2qmkvreha.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2ljatytim.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2flszqgzp.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2nuwtizhr.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2dbrrdpmv.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2rqyjajnb.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2pfalkndu.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2zpjencxv.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2jjevsyeq.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2xcvifarl.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2pgjfgeis.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2xwxwvmmb.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2nqcrmtow.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2yoeflbos.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2dupjlsyl.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2fhwzfzms.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2ccpibjtt.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2guknvcbh.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2naltejgn.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2vrwsblfz.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2khkuwrhs.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2dlbwbgcp.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2gjwsebtn.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2dwattimr.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2vwzyywjw.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2gjkwyjfx.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2awekettn.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2qjdwlzhw.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2jygdpvoe.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2lqwkcxdt.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2iyrqfmrv.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2bicjphoe.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2yurjqlor.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2mzrxvgzz.html


<!-- 参考信息 -->