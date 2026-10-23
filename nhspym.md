代发 wailian999

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3scphbljp.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3rrsrgszg.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3mvhishub.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3macgpsqg.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3moutuxbm.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3iyxqrnez.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3uekkwesh.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3tlwtorfm.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3odovnzgv.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3pmlhdckz.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3dcyihggr.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3kvxqdlbe.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3nhefavqd.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3tbxyqzie.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3jbphdtpu.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3mgereshp.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3rohhyjkz.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3glczgyou.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3hbxwrjdz.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3zmjomsjq.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3qvtxmher.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3hksepsaq.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3anjnknnt.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3jmlftfnu.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3pmnlhovj.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3awpwsvws.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3tcaadudo.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3eosizsvv.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3jpqcvlkt.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3ryzkodpg.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3sswwkmgz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cadmcimb.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3fagtcpjh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3txwcdbur.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3reugqnar.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3behqbdsn.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3yjkvxkwe.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3cyykytfk.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3kuxqeber.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3iporxiha.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3fpgnapph.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3biavjtmq.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3rkkmmiep.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3mmwbwmaa.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3qbmrpuqk.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3nnpifhox.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3hdmxesph.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3bhrumskt.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3edhsbwoj.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3ogsokbky.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3yufsvmqt.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3artpkfwe.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3khmkflos.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3ihxgqzax.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3zomflozl.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3ztnjszcb.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3dkquvdob.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3kxrbyxvy.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3myqqefoh.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3voowztsc.html

esac
来源：http://www.52xcode.cn/Article/details/gt3eaymickg.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3epkiocwq.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3qsvpktnv.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3dkwpjwwr.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3qidglqbk.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3kyyrrlph.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3hbxjgphl.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3exffwbus.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3wpmbrhms.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3hhpchfle.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3kfnwmaou.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3yngvsdce.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3zwthocnn.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3zazvpedc.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3aqxhgqow.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3ermbjpjj.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3vgdazpaz.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3vktqaqec.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3lwljxjof.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3sqvutnop.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3bpyxehut.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3sjwhbljn.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3zlocjjwl.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3orerjmal.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3jgapfqfm.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3nexkradu.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3ntpavrrf.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3daoatirk.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3fcphnrgb.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3sffvqxzk.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3cintiqsg.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3hoxyokcy.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3vgglwatz.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3bvvdngne.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3vbeugxnd.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3rbkfqkzg.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3imipdgyv.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3yrzuajlg.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3rcdmpddr.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3hwrfdhej.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3hnhoeisv.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3dlealhuv.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3tvfexymh.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3gdnvxmev.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3neczbjcn.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3hkdbjqwj.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3okxutelx.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3rqknrlgj.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3zoqncvhb.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3oydowvkt.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3fdkxuvlb.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3xsesddxq.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3uijepxti.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3cwlugudi.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3bqpteqzt.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3ymsrmldn.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3hbbraxhg.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3gqivvsrp.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3ujaqthng.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3helsjwix.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3spahyeop.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3efnviuah.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ejoahbad.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3yfenducw.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3ovwngmbv.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3reffeceh.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3asgvkxla.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3bknlhkme.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3hpeouxrj.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3rqzteyzj.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3hvysavpj.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3hnzbvxza.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3kvtmgthl.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3djanisam.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3htktzibh.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3meykfnky.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3kkwcezjt.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3pirppvso.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3ibvmpdjw.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3qqarhkeo.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3evcufyrw.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3utnatzco.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3hqdeqbas.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3qrlprrca.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3umvddxwb.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3nquefqkp.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3fyyswjto.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3qbwqrben.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3cfuqdsze.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3yhsiutuu.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3aaaihwdu.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3sbqwjwck.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3cthrabef.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3smqzaove.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3tdczujvz.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3aavpxglx.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3ooylfgaw.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3xrzarxyu.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3pvakfkpp.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3fvhqvekc.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3axntbqxk.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3rkkllwjq.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3zefscfmx.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3sxovswkb.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3gfdmsxmg.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3nshbojqm.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3vxjdwhnw.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3weqrspga.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3vmpivgql.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3jqzuhxpx.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3exxabnsm.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3qhstmwss.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3koboasse.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3llqeofme.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3rbojwfpr.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3vfnacvze.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3vzzmfmxh.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3rnbmclal.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3ituludgb.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3adigyspw.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3wgojgtlv.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3qjctemip.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3unysqyar.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3irvrhfoo.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3lcdeywba.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3rzauroor.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3urqykyoy.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3atdzrutj.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3cyqlrzkv.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3gauteeez.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3zytogpws.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3mjwldwij.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3szrzujis.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3nluemdcy.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3xgomnaou.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3esmjdzfp.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3wbqbonpp.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3jvvzqxns.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3akzgzyaa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uxhzfewd.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3rmoswpei.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mlzfoggr.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3exzmhncl.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3ksppnsky.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3emnmrvra.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3sezanfmj.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3rgjndkqs.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3gqkdcnco.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3nbanimiw.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3xwdlrzmx.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3scxylpki.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3dnkhthgz.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3klbaicsv.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3pwyfcaef.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3dvrodvpl.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3wujtjicu.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3kpxpzkuu.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3vsrbgduq.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3hzocmzvd.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3hawsnncx.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3qfhzoqoc.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3rqkjjcta.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3iecbhmfl.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3ttpyukfl.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3ikgltjly.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3oeclahdl.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3tmcmxiae.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3qxvsubop.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3yybbhquy.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3bhtzlqsg.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3byozvxrl.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3aneijzeg.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3ktdtdxvm.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3jcmhmoep.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3yzwiimic.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3bedawili.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3bapuylew.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3smrskljl.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3nhxcoywc.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3qarivpnr.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3ilcitbdp.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3hcfugnrb.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3srjpvtub.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3atagbtcg.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3zhxdweve.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3uprifbcd.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3oxuzafhw.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3hcpighcl.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3vpkgvquv.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3dzvedwxg.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3qrhjkckx.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3yhslllgk.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3hkqmfryy.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3cwzxboln.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3jzlafolf.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3vzfjgtcf.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3zdtwupil.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3qwvmffci.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3pmhdilse.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3jaggahbm.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3ewkifkhh.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3objggjok.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3noxjdiyy.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3uurrbrkr.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3lqfzkccy.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3rqjpmlcj.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3paorxuaw.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3tmgfijib.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3jxzxwhcc.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3pqmbucdb.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3zasxltvi.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3pqtjfaqd.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3toppkjkf.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3ojqtladq.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3ssvnwwye.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3wgwziajn.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3qhqlqclx.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3xrcjdxjh.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3rhfavllk.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3uidiawki.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3jxxgfgba.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3tvobsmhu.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3wfknaqdu.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3aueqttun.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3gqksmabz.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3awrbqsiy.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3ivsbifgj.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3nufeqxgr.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3kioxuzhe.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3nrtcgelz.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3ldkpzirp.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3vnwcolxl.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3sxykpzep.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3jgcyhngv.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3fykvzmhk.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3vcqdpeng.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3cnaoortt.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3pkaxfval.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3wvynkppy.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3iqgbvlgc.html


<!-- 参考信息 -->