代发 wailian999

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3abdhmbei.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3hmogpfze.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3bodkttdb.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3wdhtqjkh.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ykpozsbm.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3hiisgszr.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3avvfexbv.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3iwbfbzpe.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3yfcenygq.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3smycdfkd.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3bjdjfulb.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3vqinimcc.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3loenztdg.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3jeanfqgm.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3wysfkcky.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3sxcjgzaz.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3ucdsbebo.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3moiokjjz.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3syllcwcv.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3fjfscgry.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3uuxipqce.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3cqtaqzsj.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3whkssxxz.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3cnxadidf.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3wvghooul.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3kgqligor.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3oqsdczzr.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3xegsqtwk.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3lvtrmpnd.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3snmbksnu.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3wotjlviw.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3htjdpsac.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3vahaaokf.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3ronrussg.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3letlerva.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3wfhcixzj.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3vvkbuojf.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3ggisoczj.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3bpkonkqn.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3ibaxzoer.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3mqckadcy.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3zrsoiyxf.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3wpqzbahp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ljpdejab.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3hntkyyil.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rfonnvbt.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3dknkskoc.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3xswusiwm.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3qdaqydjo.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3dfhwcisd.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3engqegna.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3kuckntha.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3mrfahset.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3lvnfyjgg.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3pmzjrdms.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3onhzpblp.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3lhynnbqg.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3abqnmlki.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3qaedfrpd.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3pwniklzy.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3lpdlxima.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3scktxgtx.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3whgkdymh.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3owsswpup.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3qseryezh.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3klylzevf.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3ymvjxdia.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3cjyknxsk.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3quqziieq.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3fhsvefbj.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3zpkkokck.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3cypmwvgc.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3tryeeffa.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3rekrgmee.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3vxdzzhmg.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3gcjzvsqu.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3cvehvnji.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3qbryqqmz.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3pvrptfhr.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3ebuogczp.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3jfihhmdu.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3ohapeine.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3oingzcph.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3bvszhumc.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3lsdkjzfz.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3zxwvwkef.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3tznqljrv.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3cfgirkuf.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3tzkjabsc.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3ywhtxgts.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3pmkhjetj.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3bmhgudor.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3hsbkyptx.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3dpioegkx.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3fjitwdgb.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3qkedrffq.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3ofoiycep.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3qabgvdvn.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3llzjadim.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3ekebjcvf.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3ywmluhhz.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3qcdknobr.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3cibxvyno.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3jddkcccl.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3iakihqzz.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3knaumxrb.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3yxbyybjp.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3mzhwcvcm.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3qweuengr.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3huhpjpce.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3xavsillw.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3mquwafmg.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3nnzpcmrp.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3caqvdnoz.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3rtbybrte.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3bjtcvsxn.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3bfdwlpeq.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3qavxhcnm.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3smmhzypu.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3rvlqsuhp.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3genzyvbt.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3fdsbuogd.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3wahqywcc.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3tcoiqidh.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3yheriuxk.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3dmvlzgjd.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3xytlddce.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3eymncgfd.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3gqvrwuvi.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3eomvaaru.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3iyhblzvq.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3fmrmkggd.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3cptfrjko.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3mbagahmy.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ntlhyxiu.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3qpcpbhgd.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3mdexwsul.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3nlfbknhw.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3uejbfxmf.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3rvjinupn.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3niumihnr.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3dgxgkpiv.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3baapdjkj.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3cnnqaigv.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3delbhtbx.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3nbfkrjyb.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3wgejgpas.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3xanpxeyk.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3rgnsfszy.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3ucqbbvkf.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3vmwkapqd.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3pzqzgwjj.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3qlecfsbu.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3liyuyfww.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3lgvbdchk.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3txjaazfl.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3fchtdlyz.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3henzmwpa.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3uvttubxw.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3wfndldhp.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3kbaaugtz.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3zldrczut.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3ycqpkuat.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3tlpfplwl.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3fzrnbqvy.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3almdhqvx.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3wzurbmai.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3izrhtcku.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3nzdxudrc.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3nswikkat.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3uufkryei.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3ubaazzqi.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3wzegrsze.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3aebdijfa.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3rukuhcsm.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3oudjmkmz.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3kivubqxq.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3nwgpjaoa.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3tcctrhxq.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3kupbwzix.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3bjoxzymt.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3akmxtywa.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3jvusxsfi.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3yjkhhand.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3pghgmucg.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3taxqtrxg.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3egilvbjr.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3eicpeifz.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3htxzlobg.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3rjmrudsv.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3rznbhrzj.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3alqhfimq.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3upmjhgmk.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3cuqfwtbv.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3wznikwiu.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3svntjjyb.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3lvdycdgb.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3rcdutcar.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3rhwudvub.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3asdxsjjq.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3jfgtaivk.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3ekbwhbsx.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3lmixvdrx.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3ahdjntnb.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3yohzdxty.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3yjahxoiq.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3afvahkbm.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3itirmqyz.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3ijnnmlld.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3szhqvrmn.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3mtgnvish.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cfzqknwg.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3textgknf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3krfscsrn.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ukwsmabr.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3aofjkbkh.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3urtuwisx.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3uxvciokh.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3llioqcsx.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3kqnsdxle.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3tdjhteog.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3gcpdztbj.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3acwgusvz.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3fntyagpq.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3ecvvpwcw.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3yglwhbyn.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3pguushnn.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3kfbgxrcb.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3sowfskta.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3rzqbsxrv.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3bhrgusco.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3eavlkvzh.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3iuvjnkxl.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3nbmudxmr.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3vthqwngn.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3tkicxbez.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3gusjgpbt.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3ssgusbkx.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3fhcuwbxl.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3ijqvazyh.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3ruknodol.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3fddjuhxa.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3cwgjaoqk.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3qwkedizi.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3oeldrsrr.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3rhqullkx.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3smvdcoyb.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3sppwbadb.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3hbaqqpag.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3tgtvwcfu.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3kgrgjlyq.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3zssmcldr.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3zpixhuqf.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3pvrjrfwy.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3dbvqjbdl.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3qvecsopd.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3gunneiyq.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3nogvvstr.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3eolwbiin.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3ptxhbdtc.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3faqjqsbg.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3tleouizh.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3tutypqsb.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3trljvjbh.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3mvheaupo.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3pgjikqgl.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3nmegnfpq.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3aewlsczn.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3cxdbtrtk.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3cyeccydn.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3inngygak.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3delbwmri.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3rrvurxbq.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3nndqmrzs.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3tqbwycgx.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3ekwrudry.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3rjrkstyg.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3wohdwznc.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3bpycvibj.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3rqiqnqep.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3wyeiuhfq.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3qpwwkfjb.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3acytuiff.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3jouudmzv.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3rfhqhcfb.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3oyyedctz.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3zmwcesgt.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3kxmhjkbf.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3vmuzbbbe.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3rsjfvwda.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3hecrcaxx.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3xbjjhdoh.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3lztudpvg.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3nrsrvvqm.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3yfrhfrud.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3vbxdmlup.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3dodgrdna.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3fxdojdlf.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3btzsbugt.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3wcrdhasq.html


<!-- 参考信息 -->