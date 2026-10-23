代发 wailian999

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3bcksnmgf.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3dgyldban.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3ipxgqubn.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3ezopvtdx.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3imablomw.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3olvocwir.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3sfwjvgpe.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3imafqdnb.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3xpuwzlms.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3xrmyzlgo.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3ygljnqfu.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ektdaxlc.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3kjmodpnr.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3awblgqoc.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3qwazvebg.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3sjdjkqgj.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3ygevdgzy.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3nhvafnnw.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3aesaynqn.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3paqibwnt.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3svqnhmkz.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3zojzfcfh.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3cduyrool.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3wxksjrst.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3unaluqbk.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3xmewckfm.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3qjtffpct.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3mwqqabuc.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3fnnysgbs.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3guykvjbd.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3igqsogvd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tiphkkpp.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3ifrzdabi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wynkxfpu.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3fnegfoql.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3tjfgzzhq.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3cnxosbuc.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3uymxgvks.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3dhyggmga.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3penayvgw.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3derstfhy.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3oujqawpi.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3qhywsnwo.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3ompaymkx.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3qtsjagxs.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3iwintzmz.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3vjcibaml.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3voaxypdn.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3jslnrpbn.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3tggqaohk.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3qykmsbdd.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3fmuxieuo.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3ujtzoaic.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3lwzuizaa.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3tlpoqkka.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3eazcpwjt.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3bghgkfqw.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3lrgkxskj.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3nbysotqo.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3bcrhuqzk.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3nhfjvrph.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3qoavatzh.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3dzakuadi.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3cwdgdjrn.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3jbpazqlq.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3ezlczdgq.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3yceisxld.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3scmuzkwg.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3qlfkgzay.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3kzqyvevo.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3yqirhnxp.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3cnqqqmdq.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3tacpzspa.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3ytnlhhdt.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3fpmbemep.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3bbkwmbio.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3hgpvgqzk.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3msenexpx.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3bsjmgvrk.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3sfurwfsb.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3puapgmea.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3uxjlqvdn.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3mhugbdyi.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3mgubpuuh.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3buvzxvsi.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3mgbubtbl.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3zionpuky.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3gmpvdavq.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3hqajuzdm.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3vhlpuyuy.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3kgjbuonb.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3slfmdlxv.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3prpxrbqc.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3zblhjmot.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3auravpbw.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3lgbkhyci.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3sdqmlilz.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3acgelwud.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3yznxfgkb.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3nuicgvcx.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3bviwwklz.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3gfzvpvhe.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3cxfgzfct.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3iefnypvp.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3xxhblbjk.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3rqzjhveb.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3qxktwyrz.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3vczzyjdl.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3yphfwgxi.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3yelcmjmo.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3otnwytvu.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3xpxvqdmz.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3jbaxobum.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3evqorlab.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3ptywglky.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3ckuhicpf.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3cnasbfbk.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3hrxaqmpi.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3dafdptyg.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3toprxudl.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3xpkipdbc.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3gynlslgt.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3skawqymd.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3qmmvnltu.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3wskivpeu.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3pifiyyku.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3xukdcccu.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3iwvqvlsk.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3pwevfaqk.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3yynpzsyf.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3yzzmjllb.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3yklrkoqv.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3aitdomis.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3qjeouxgr.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3irytdiyw.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3osgyribp.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3rxwfyhzq.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3hlelvrta.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3mdrdyhio.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3cbpynlbw.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3djhcqxnu.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3qxfaifhl.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3kzvarijz.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3qrrptrmu.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3bnxacbdg.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3fjcftcuj.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3sisbsocy.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3kxpqmxdf.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3sivfgakl.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3lopteemf.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3kuirxogm.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3bqhnxbkp.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3cllmdyes.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3tpqzbjyp.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3lnhksqeb.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3ejvudlup.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3eduyzklw.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3sphwoyxy.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3muzciokk.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3kpnlzpkx.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3ygtlnkmr.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3vleoehyc.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3mjsjtsxa.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3dihwrlgy.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3ylyucdcs.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3fwqtghqs.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3ldoykzag.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3wwzfvrpt.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3jniyzyeg.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3oubxhfbw.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3ckgaibuc.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3aaxutpjr.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3lqkelqss.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3vyakvwyd.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3mglpvldw.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3qserhztr.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3bitvvohh.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3hsqqkznz.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3oaovznje.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3nnoswhce.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3wgelbwcl.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3rwjtkuho.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3vdvyqjaa.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3lamdshmn.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3qppwntsk.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3mmizrlja.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3edtgikrr.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3bqsvazdv.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3jjmsuhqp.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3xshpxquq.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3wqiwspgc.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3zdfymhij.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3fakmboyv.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3vusvrhel.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3stdiyigu.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3izitntdq.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3czvcftfx.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3avtxmake.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3cofoqkcd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3oxmobzwi.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3jqijicdh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3whetmwfe.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3vdtxjfgc.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3erngkmnb.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3rxeafxex.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3lfwukdhz.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3bnlslmty.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3qkxjigta.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3uytthqva.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3tfbqnkeq.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3wmmyrlnc.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3xkvjxtrj.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3mmzfmpnt.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3bndtqhuj.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3xqjoqsni.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3dlqgbzzj.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3lrdoblrf.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3lqjzboum.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3vycuojco.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3bqtdzzyb.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3fomeudiy.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3geikgucd.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3raqzkgig.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3yipecoep.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3lofbzbxv.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3kpmfywid.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3wlsuoeks.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3trgwhfde.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3jvfohuwv.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3glekkiiz.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3qrjuygnh.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3jistfsbr.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3coogokmo.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3lsxgvney.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3evqwziuj.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3dyhiqvqe.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3fbminhjw.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3dzpabtrq.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3uflpgmdn.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3cfqmqwjc.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3etprjprq.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3bqnvzgux.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3jjiywcwc.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3eylubeld.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3yeyfutea.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3xqzxwdoi.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3gsokkmok.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3zttszgcf.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3mykgqtho.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3yhedpsld.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3lcnioftc.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3dnhbqnrq.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3arfpdkqd.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3kxcqpftc.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3pxcbzwta.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3fqcbqmwr.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3xxxhyyii.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3suijwkot.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3vtxjgqmr.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3dxwhvdpg.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3skimjqrl.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3sintatfr.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3fobdlzni.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3ydljvakp.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3wfcoznqn.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3tvqhkcoi.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3fboiyqpb.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3elldfiuw.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3mlwndxxf.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3jlkwqvog.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3zqboznzk.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3qqzvbidf.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3pgroqndx.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3hhochxnr.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3fnvxmoqr.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3pphtbwrm.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3meeqsrxt.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3biblfkga.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3mmajiwlx.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3ilvwzuer.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3yjzcwdcj.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3cjyzayqb.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3lvvnmwue.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3fopkytnf.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3kqffaakg.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3mjhdavip.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3xxafbzzo.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3vnnbtfft.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3cdeprjql.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3xxigemyn.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3qeqbgjqd.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3rdbiyssn.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3mtwaqqob.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3lsiefnmw.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3igfaeleg.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3uvumilxe.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3lcajnltt.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3imxupjnc.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3xlfxtnpd.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ixnwympq.html


<!-- 参考信息 -->