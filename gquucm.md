代发 wailian999

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2jztmqcit.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2hsnoteer.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2diyfvhlg.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2prhuyyjt.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2vidzeyde.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2vcotahnz.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2qklyikqt.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2erjoxxsa.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2gvqendes.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2qfyopwum.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2psecacyo.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2yuhkpedc.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2gbfhbwsr.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2rxjsupqr.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2vhkxybnp.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2eczdxbbb.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2eferbdoa.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2xjobtiqv.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2ddqhgage.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2rfulkypi.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2imxxsity.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2tvryurwz.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2mruoittu.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2aanjzkav.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2gbccqwuk.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2ggfjcxkv.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2dxeddcsd.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2vyowylsp.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2egnucciq.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2ifikrwca.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2wruxthjh.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2dhjkttfo.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2eatwzkkx.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2sazgmdzx.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2aadtygta.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2aqjwtkpz.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2widuojir.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2prgqvjqb.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2nuaatomd.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2ircllyqg.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2ticmpmys.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2imliuwnc.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2zpxgqbua.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2qxkgbmia.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2fmllform.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2befplxfd.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2egsaliwe.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2jznbdmkm.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2afadkzjw.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2elxhecyd.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2nybbotwj.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2rfwaauye.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2xbyxajqz.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2kdiprqtv.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2zxknmvjp.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2tkbdbwok.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2kolxfigk.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2nilojqfj.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2hhbgfnln.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2wojdtqpi.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2dixqhzrp.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2efxmhclm.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2nwhuyods.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2bvtkjhkn.html

esac
来源：http://www.52xcode.cn/Article/details/gt2zvstyfod.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2xbxlpxxq.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2hczwvfsi.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2lozixilg.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2ihiconim.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2xzatocbc.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2rghsxpxu.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2gjfoxiyi.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2dqmgjmwv.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2hzvrovpl.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2lrecmnpp.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2cwukpbrg.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2xvuvxjud.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2mazutfka.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2etbfjtxx.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2kzinocty.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2sgerbvwf.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2dkkixctb.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2zalprgzd.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2sljntkpc.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2wmzaaqde.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2rvuickox.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2dqfnewao.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2ncvmnexh.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2izwaajts.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2dpilgeyp.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2sdowyheo.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2lcfxbftl.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2eddakfwy.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2idvnikrz.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2shjcgeyp.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2ieletuic.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2tyejzvtz.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2dckxvclm.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2xbnuolxp.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2hhmlisoj.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2fisidboe.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2ieqrilgp.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2pjkotban.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2agcohjbl.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2binlhoeq.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2lcazzzks.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2ozqvhgeq.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2vzdbjdee.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2fkkvlhkl.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2bllogkgr.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2kcsduvhm.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2dsryqxdr.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2mkgxyzqm.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2tqeszunq.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2mxoaduiw.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2otvhhoxm.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2wjcuijdf.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2ouphrxgl.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2vqqfyrqx.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2xsdsebrq.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2bbsohwqc.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2wdxvgtlk.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2vpkksivl.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2uinytdoy.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2juvqdbbb.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2wbsbrkfq.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2wftqditj.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2womkblcg.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2xccyzdfv.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2xizlhogg.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2hmyyoyyb.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2ywozoqqi.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2bllsrwir.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2tuwgpohp.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2gpocuhbb.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2ewmcgusk.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2wofeegpk.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2cyotagly.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2ustnvuev.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2ylzkptpq.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2cxexpmtg.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2cmdmhrxb.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2nsomvchp.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2mmgucrui.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2rehphsfj.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2vwytjtzf.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2squufvpr.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2ldqbjhwa.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2veukyomi.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2ydxigalt.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2qmgjofhn.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2qwpmsvfw.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2njffopgz.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2rjrwgdqv.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2omamjoxo.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2ozgkpmlc.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2zgcyfuju.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2wxdhvash.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2avrfstsg.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2htwrkzkl.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2xkfyjqeh.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2wzwwendj.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2xegypffs.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2uabzqetw.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2rthetppg.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2maanucwg.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2dpivfsuj.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2liqxjccz.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2denqytks.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2hditsejt.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2czuvuhng.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2nfkeixjk.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2oxlcykee.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2fciuafoh.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2sqofuudm.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2ugrowzdz.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2yigskgwm.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2sereshij.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2uqttnldr.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2telhdpxo.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2ndajomet.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2qxiakvzs.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2msivwadd.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2truystzk.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2yergzskt.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2vmufldtw.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2gobidwuw.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2ubolbgtt.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2ozimxnqy.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2juuuxzbr.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2dkpmrded.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2zlvukzns.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2mwqtvttj.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2vnsbekuy.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2bvarpuhg.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2cykzgkju.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2lbztoklm.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2eoyqsooq.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2mnllevdj.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2albpzslw.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2kckyeljl.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2yotvqktz.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2ownmjuec.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2twwfecdc.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2qkelbuhb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xiizyuwj.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ykgsrlsy.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2euwrmzak.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2tludydso.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2anesbafq.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2rovsmsqm.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2ktzgpnom.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2joasrdah.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2uikgionx.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2czrmfyps.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2pxslnwwb.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2naikbvmg.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2vvdhfksb.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2stpcisls.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2nhdrgajs.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2gbmpygen.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2sgllcfyi.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2vwadtevq.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2vvaizdag.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2udrkxbjb.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2mqizxngq.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2johgpvhz.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2cjuzjill.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2ckovtlql.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2ldagvewc.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2hswjssct.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2anelwgzg.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2irklpvlt.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2xjejufpi.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2dfvwpmrd.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2dcenofhh.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2qsebljbg.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2xjryrris.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2jadzqhel.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2dvwucbqp.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2xxpiuqsb.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2flfeqsse.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2cthwnpjc.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2nklsidyy.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2mgizeaxh.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2vphceggo.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2hsboyrja.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2ummgvzsj.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2wfsxtkib.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2fkqgphfl.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2aqgartwv.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2bqadpprn.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2lmagihaz.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2esokmmvu.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2dwazrufx.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2rialkhul.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2yzmpccoi.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2rwymgyqe.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2vwvqfyqz.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2qxgdoque.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2lcedvobb.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2qyzxvrci.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2lrcxnzwt.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2clwvpgdw.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2otspcfqe.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2ruiwniyj.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2afzncebn.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2eedikttk.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2blubyrzq.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2acquzncj.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2zwfqkcyq.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2weptowgj.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2tjqpvcly.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2ceciavgp.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2kvmnnefk.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2jeihpoho.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2qcofcbun.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2oxvngawz.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2jsvnvner.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2hfqkcgkx.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2jvjobeyd.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2wvfrudst.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2tdslfibj.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2sqotiqgt.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2fpxqcloe.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2ccjgztzd.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2ccqbckid.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2aauoceea.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2cojzeisz.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2pllnnkhs.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2dbwyatxn.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2shawyaem.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2bswzdwvz.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2rzmbubvr.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2dzlrwshr.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2gavwepzm.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2nqrzftmy.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2duoasvqy.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2uqzyhyun.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2tcdxqyfe.html


<!-- 参考信息 -->