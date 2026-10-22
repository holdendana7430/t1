代发 wailian999

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2jcxqpkww.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2aluybjkh.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2cepofjrx.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2tyywlcox.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2sqziqtez.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2vokjfazl.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2gwgplqjm.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2nbrfohwr.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2odguyuye.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2miuvooct.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2galldyce.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2iyyectmk.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2kvwjyjeo.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2yrlpaewc.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2hlueescu.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2dfaiwxnv.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2gpsuorsw.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2ujlzvmyo.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2sdrwwufg.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2spgzswxq.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2sgqhacaz.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2qgohykxd.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2xvgbxopv.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2pknsuikx.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2iydppfdy.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2dkllchel.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2zbrlenxm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2oaiccdyk.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2vxloihqj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2phdxmmlo.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2ebcqiyie.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2rwvygrbk.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2bxtkvxaa.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2mdubpqhz.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2xpqqfhlx.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2yeknlzkb.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2eekhwvng.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2ruiodkmh.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2dhtzylyi.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2zjqlsyfw.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2ivbalktg.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2ntyqwdua.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2ciuximjw.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2byuaetjp.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2pwfdspqz.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2gumeaffn.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2ubhwmpnh.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2gcclxust.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2fizpuxdq.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2ocdmdahj.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2psvebrbv.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2eijygsig.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2otkpvwfc.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2gkfxfkzw.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2ywtupfzs.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2opommklu.html

esac
来源：http://www.52xcode.cn/Article/details/gt2odweyhqd.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2vandtnzw.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2qrukrrge.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2bejlsvbj.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2mocmypre.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2hnaqzeqt.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2lnzqhzji.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2iduklnoi.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2ezvzdyrx.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2qitklxaa.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2jmejashv.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2cibhihdd.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2zbhbpzuo.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2xlfwumcq.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2vhacvhjm.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2qacsbasz.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2msuhkqni.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2xlaertov.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2dwmviish.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2rzvfnxvl.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2chkswcgh.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2nbnmjtew.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2pntzssjm.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2xesqbspk.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2cpqrptfk.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2dijxykko.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2itxdouwm.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2uhbvanro.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2zqjhctyf.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2ekkvxguo.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2jvkquiom.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2yqfmrdew.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2wbtqfxbu.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2fuubkaxr.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2vbxkmbqj.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2vdlklvha.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2lwbqdpmx.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2vkdtjkob.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2cyeicamz.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2ckogsatr.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2thqyqcrf.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2zvoulvbz.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2fusztlin.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2lawthysb.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2opcazqfm.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2dsyfwlee.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2dozauqgg.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2zbiutsnw.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2crqjebuk.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2mpnqqjnw.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2mtfoxipm.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2aonwoncn.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2ykwnviog.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2ewdcqzlt.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2bdtyrfkn.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2rnurtahd.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2rxysfybb.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2wzzdnvfc.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2zunskchc.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2zyjuzuxh.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2kixupfcv.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2ksdtjvwx.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2yybbatmr.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2yfwejlnw.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2osltehku.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2pvahqiyk.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2yxvyudcg.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2dmqmaowi.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2ovhebzuq.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2rclmsick.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2fsbqdkqc.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2vffwyeak.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2ywsnkdwj.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2jucwzatf.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2pldwahhy.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2zpisrats.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2ktnzyrye.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2ewxcamnk.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2qxjudfzy.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2ejdevqmj.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2biuetyyj.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2bfbryfhn.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2fvarwxfq.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2okespiiz.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2miecnnnx.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2zrdtyizp.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ooyxchrl.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2rsjyjolf.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2rweagyki.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2hhmiulzh.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2caqzshid.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2hwqavayo.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2hhpqdzjc.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2vtsalxux.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2cyakebao.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2lkzycpov.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2hqunsqok.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2oyudurlg.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2qynulejf.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2nmczoqlc.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2sxqnzkoe.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2zbbhcdqw.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2qentgjtp.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2pzfhzcwt.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2jpotadja.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2oxdpulai.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2fdfifwar.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2defloeod.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2qnwufzrq.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2wwadaliz.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2vgahiyqb.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2doelrbpw.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2tedwptnu.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2rrzofmkz.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2zqvdwvfk.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2yoezziem.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2bsedynme.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2yzyhfego.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2gxnchpgk.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2awdhptmg.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2tkfoaccp.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2yefkxais.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2jgboduls.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2arrkwomp.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2bpeknmmz.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2vlcvqnwy.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2vmdgnwyv.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2zoeqghbc.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2yeddiubr.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2ujziyrub.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2znanixak.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2qfduesaq.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2uykwntfz.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2gmpqkppt.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2gspoendo.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2uwtydpyu.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2aumgghhu.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2aqjbdguw.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2awtlklel.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ycfbjsvo.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2qzywygbc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2evuolvzr.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2bhuzxygu.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2vahlbnsm.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2enyqyzor.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2ecykhwoq.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2cxvhdrhy.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2xqiptpcv.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2fyqoikck.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2gahezptp.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2lghemcmq.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2grunplpc.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ulkqrimw.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2dfxsphra.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2kxftsnuo.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2upokfvrh.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2kpsobflp.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2qzsdzyaz.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2pkvqrawq.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2gligtoke.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2rgpjuwvr.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2ctltkuod.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2cukrzmrw.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2dcdhqgfo.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2bnqftyyu.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2qqlsxhcg.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2ypjarjoe.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2gimzxsvi.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2cnxcnajj.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2ucsnhlod.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2wgoiwouo.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2ylizkjvi.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2dqewyxdu.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2ugihetxh.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2ilpuufkn.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2xhtscmud.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2fsjvxglc.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2jgdehndl.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2atuphmdx.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2affzracy.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2zygbgbcp.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2vbyeqfjm.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2mbcvolfk.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2vwfdzxzi.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2hjydjukc.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2dchoeact.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2sjsxuqvr.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2ukspyknb.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2hnyaoynw.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2dcuvjeyz.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2xhtldtnr.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2gmdqaxha.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2ncudxetk.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2psouzraq.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2drwgtrtb.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2pwytgruk.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2tlftopny.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2pcssqfle.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2jwyigezi.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2gjervhfy.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2tmkjyntc.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2otgherpm.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2uiaietrq.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2lvouwhhn.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2jxfxcitg.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2euiywpuq.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2sygatnrz.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2onzhkjau.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2tlhccvqj.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2gnpyrmfx.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2qingrtej.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2blunleno.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2jmfukhlw.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2bzwzescd.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2ytpychzv.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2oydpcndj.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2bjsqhbjh.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2cldvzydc.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2fpyshktb.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2jdeotffi.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2gdokosim.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2ufleavzn.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2vamccwzl.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2whydnkyj.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2tcborvec.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2gmohfpai.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2gayetbnl.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2atbhyyey.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2nopmknmp.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2ephanmxg.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2mwdexclx.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2xrcvetht.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2qkchjmbn.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2uxdojuwq.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2qdugpugy.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2fcrsgwjb.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2qubjvcpv.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2twxwogbv.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2vwweapwo.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2qpizrvgd.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2msdvxpmc.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2zfchmpns.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2lfvydxch.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2gtjvftiz.html


<!-- 参考信息 -->