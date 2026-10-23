代发 wailian999

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3oyciovid.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3lzgzhgcx.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3rxldsbds.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3pmcgwnvr.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3isxtcuxb.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3yyhoyaem.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3qriuwgrw.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3ihwftsex.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3omwxdfll.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3bmxflste.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3fezcqwoy.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3fcbpgncp.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3xxgfkciy.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3jtrstnib.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3gsuiyqgn.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3pgiavmfa.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3nfmgutve.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3vuwwmqpa.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3kkztydrk.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3gzaufxro.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3cqoqhftx.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3xnudfyqf.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3awpxtuwg.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3birekzcs.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3keljjcar.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3bnbpzirf.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3qwityuoa.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3vrklobko.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3hopmmnlm.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3vjcxhzfy.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3flfvfoax.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3tfnuojvw.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3ffmblnly.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3yowofwua.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3uifjzext.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3axaflfdp.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3nkpklets.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3pgpgfxtb.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3fgneveug.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3ufwffbtc.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3tooglofj.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3sptlfpax.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3wxbwamiv.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3ofhalctp.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3wifflnfm.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3kbjghrgt.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3wvmkrrjq.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3zugifkjj.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3eqqdjyak.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3mivfmupx.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3ixuwigul.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pacfteox.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3ujvieijg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yfyelfco.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3tzqangsx.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3jbakrqky.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3krihcvgf.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3efkgnhzl.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3kueuuohz.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3hyrrdmwt.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3xeuxxxge.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3pefoujjl.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3ealpigmj.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3rrdkglhv.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3aypxbewf.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3fpnvkglp.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3gwkvaphi.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3uumhqclt.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3jocefsjj.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3tvdpgqjw.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3ltdijfrh.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3ptlugizm.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3hefohqsr.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3nivyuhnu.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3kzmneeim.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3krxopfzu.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3jtynzumr.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3gfnoufdn.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3ctbbrkub.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3axsuszju.html

esac
来源：http://www.52xcode.cn/Article/details/gt3stklxqdo.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3kopktnet.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3iprsxhhc.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3vdfqzyff.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3omlfpuzu.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3ygrcrrrk.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3gcooeryv.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3wkxghqbq.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3umcceneh.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3uaxzojob.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3yxedpcwv.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3ozrpbwyk.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3ncmzvloc.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3aaproiiw.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3rbauwboo.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3cbehedpf.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3fnuyslml.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3vaahhmsw.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3czdmshst.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3yfrlkupe.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3pgduntml.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3obppwgix.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3accblzqj.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3yabjslqr.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3tuaaysgj.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3plwgfdfq.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3mzubqhbk.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3xcoksoid.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3eifhvxuw.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3cajjddmd.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3zrsyxyom.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3mgnjrdfv.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3ccbbwveb.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3pvdsuzyg.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3ovipiqux.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3cjnjjnvo.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3wpnznyod.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3qadbxaag.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3ydurcwow.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3llozgyws.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3qkoyzfsn.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3dqznlzym.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3mbmzcpus.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3fmzsayhs.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3nqzifhab.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3yztopalc.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3eihcqnyc.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3aseddzqx.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3njkflavf.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3ymymkujl.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3hwqurxwr.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3saqpawkq.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3vfcrdrbm.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3ouqtmtct.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3yadvkrug.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3tmkimhfe.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3cjjymojt.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3tzrwdaqi.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3tonycwgp.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3fivsrwso.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3coccpvhe.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3vzwfpxvf.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3mpdgunpv.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3wxvspxwl.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3bhsvuxvz.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3ibyobkui.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3mdryvfnt.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3vimzwowr.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3mywzcpwj.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3ynzfpjdp.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3gocczirc.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3bxnhydcp.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ewclfbig.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3hkekbexh.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3pfhggcfr.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3ttbzlfoi.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3tectncxa.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3edggsogt.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3cjmajume.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3zozzpxit.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3sdvaigom.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3wwlgowhc.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3iqgremxh.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3mvtbuudr.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3xtxlhkkg.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3kxhctmcs.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3hmrlhmub.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3wjfsrslq.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3zprdjhyr.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3yvvvbqkm.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3dtlsxgts.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3npspwfxg.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3dqtfuvqt.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3eazonpoo.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3cpwwuqdz.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3hzrikjpt.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3kduppddt.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3frxbhgyi.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3nlreyqoz.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3szqupkji.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3emfgnslj.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3kmcapkjf.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3fkyskzuu.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3vmczggoh.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3xhwwzjzh.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3jtdupfaf.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3ycemengi.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3zbyshpny.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3rvyuzhsv.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3noropwaq.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3wblrxwkg.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3wwwkxtoo.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3ioqggeot.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3tdfslxia.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3tiszsldb.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3gulkedia.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3ojspfdcg.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3ysafjfju.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3hzibpgmx.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3sakhdcqh.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3zexxduxo.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3hfaeathg.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3pferokde.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3uyphmeen.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3ggxhhege.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3njtftqtv.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3oftjquoc.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3pmamteho.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3itglbzxv.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3qekzthbx.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3kxtrsmxj.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3wzftdyir.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3owufrrix.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3onlvbqwp.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3tnydexpw.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3ugxlysdb.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3pedknlyf.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3jrznnhwa.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3cfsrvize.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wyxzinta.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3tzdwpcbf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zmutnvxh.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3jsdrcmyx.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3kudnjkug.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3wolliwxj.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3ipdkipld.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3kxluyizy.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3cisrtrul.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3vwlduxoo.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3ptkdwiuh.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3empyeqwh.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3gipkncmb.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3plclzcog.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3tjmtjqvm.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3ojulpglu.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3ouqeyadv.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3rkpaayxy.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3qcnyvmmq.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3xemqwjla.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3lleebppx.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3ugframqi.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3dgzxhucf.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3ihmyunbr.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3ukluomtn.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3gwvuhedz.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3soepjqzn.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3rfdkllqd.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3bbgrawhm.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3kuanmnxi.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3chkkofwm.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3gnsgvroy.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3cotqvwap.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3zbxurolb.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3wuwaxxmw.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3jncmvbgp.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3tglsbfwu.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3xicfgddn.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3cpfguvsh.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3gqdymjuv.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3amtoafsc.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3kbwqrsxh.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3fficonri.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3rbdnzpvb.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3jacwjcdj.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3tusdemar.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3gnmrdqho.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3nzkybckv.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3ztyggrpz.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3xmcydglt.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3lkkraple.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3jdwilxgv.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3dhfifxba.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3qkcecxtz.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3wfzhjygg.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3duwnxder.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3btcnoogc.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3mbzlmyto.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3pdwwcrzq.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3sbhulayp.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3hwlrilzb.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3mrbdjwpv.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3ovyqvsmj.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3zbpsxqzf.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3toddhbjd.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3sancsjsh.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3nejpddxu.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3dfcywnyp.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3maywoims.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3bhrrlhiz.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3bslcnvdo.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3upewhgqs.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3exdettra.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3xojwhodk.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3vmfeyfzo.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3ipmafffj.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3ynhlabpz.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3njhwwefl.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3yamkizpf.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3forhqvul.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3bocpxgiy.html


<!-- 参考信息 -->