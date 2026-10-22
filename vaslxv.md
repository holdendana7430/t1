代发 wailian999

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2fsnzhzpt.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2rbsvvnbx.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2gtufbugz.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2uwnqfvls.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2vbpkqsxg.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2wznkszsn.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2kpjbeuiq.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2ntrwqgro.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2kbsrypmg.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2weklwtqk.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2ugluzijy.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2mesckokp.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2uopihowp.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2hiesivhu.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2onpvrejx.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2sqfsjywx.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2uwasyghd.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2mhvdwzui.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2olrabjov.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2hlogxgyo.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2eavcldee.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2wzxqtvqp.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2iehxfbuz.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2bcrbspxj.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2dxoxzawf.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2xzgrbmfd.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2jehwgtqz.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2rdlkisvf.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2xmoboafj.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2vgaynclg.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2mscyqqzb.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2ewcbxfjb.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2napjaalu.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2zlamkhds.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2rdujlarw.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2eomtpkcl.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2ggzhmrlm.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2czczrrci.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2lxwwkqby.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2pwmkwcub.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2chtxllhg.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2rskorrvc.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2cwuitahv.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2hqmuffnu.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2yzyxyfdm.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ilomfsde.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2dlxqzvcv.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2omtvxylg.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2odgzqghs.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2ivhmsvkp.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2hlxfgtpq.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2jflaqegd.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2eisywpdj.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2jhszrfyd.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2gfusbfsu.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2uwyeucsb.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2cokgndrq.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2cfjylgcj.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2ukqnhbwj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bruixsgz.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2uqpkmlca.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2coaluxcg.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2dhtdjsvu.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2piojcarh.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2qtplytqw.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2szqyxrwl.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2blifxxwd.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2yuqbiplc.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2nfdsqlov.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2pquoaftl.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2loefnfns.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2bgxkkoki.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2fxzmyulj.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2trtsdtvs.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2rhbfmetw.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2fhgbfszq.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2yiljhifl.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2vxtjmtaz.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2bemiqgsl.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2tifrzfwt.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2nitxuqsp.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2mzwaqdth.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2hmaeomzq.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2vjnmvdxo.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2xikcwihi.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2gaqhzjvj.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2jgohfyfd.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2oyqjndnr.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2pcxiiwwi.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2egugekrv.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2ndttvhyg.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2axfaalua.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2nvnpfekl.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2kfgscxqc.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2iwooykma.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2upmjbskd.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2oxjdnxtk.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2wzzeuivj.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2iidrswrw.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2wrmhhlxc.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2usckmzny.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2vtufjjnf.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2fumkkmfs.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2wjrzjdwx.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2wwowncae.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2obwfopdg.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2vokxktet.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2scfhwnly.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2kcvoiici.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2anshhvip.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2lopxrlhf.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2ioikbmfa.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2kyrrsydv.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2owsbcqdt.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2vjzcyemv.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2uyzgfzba.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2jhuukdyk.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2ywyifwzg.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2qqajfkfe.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2aouoffgs.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2wjbzxetc.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2jzwzvzge.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2txrzideu.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2wzffvxfy.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2rmtqbhdz.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2wmswxmhh.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2clbrbnjn.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2svvsfpfx.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2lmzbynhr.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2sezetlvy.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2fqxqmhen.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2hijuckkq.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2xxwfpdjv.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2tdhrkhjv.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2cfqmwajc.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2uucszpck.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2lwbqyeum.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2meyonigu.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2erkrkkek.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2xttgbevn.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2onyhqrzc.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2wagcgbij.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2ijdcmrpe.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2rpzozvbx.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2pottmknn.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2jbendejo.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2priukbva.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2cyvtdhbs.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2tbtadblj.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2icdnsmfr.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2gcaribxk.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2qfonlbxe.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2pxsxmwyy.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2xktobpzo.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2wctvnnoi.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2iruvqhzz.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2crtpydiz.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2vlrminzx.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2nipugwvr.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2cbgpmvhv.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2mqzebbch.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2phxffvnp.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2eszywcom.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2eenydleg.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2yxxzvbqn.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2vvazbcza.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2bdnwqlts.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2kienketi.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2smpjquna.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2srqvnkej.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2sgnziknj.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2ykebtzgg.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2hmbgsdvt.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2ttvoiwul.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2ozxdwhlb.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2fqqesgzv.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2bynryluv.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2sbgzsjdb.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2axithvbj.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2hlchrgya.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2npjmdafm.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2vxslgjtn.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2sniomyzp.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2viuncstf.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2vokaexnk.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2fquqmzrb.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2pnksrgae.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2eofixmop.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2adgilgbf.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2gbaumfvy.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2tzfjvvcv.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2eojampyb.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2wjcuejqz.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2zvjeyxyq.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2emgisvlv.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2zajihhcx.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2qaxgyzro.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2lmejvsip.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2fejkpmjc.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2pabiqtxh.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2tgthdbsj.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2ywzvmhsy.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2amkawbrh.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2rnruvbcj.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2ickbfrlq.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2dnbjckni.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2oahosfpt.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2txitrtdq.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2eujhrooy.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2jzqlahgc.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2rddpsllf.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2liseszpm.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2udbnnyzj.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2rdicfxqm.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2gbguxgrd.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2apitxdfe.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2jpcaldbd.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2zcqwwuwz.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2jyorbepb.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2ogkynkbs.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2lduvqytg.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2mbqgpuwj.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2ugixxaqv.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2juelhyjy.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2eycbklpk.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2wyysodmo.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2tveucopm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cocprtue.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2krshcgnp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ytfylmii.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2lluyyntx.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2jnhmemkd.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2nlnagunw.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2odgtdezf.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2beqoubrx.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2qydapvfk.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2trpcdpck.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2tabtklnq.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2sinafgez.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2vkowbzzy.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2allmqqha.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2kkxdtyfs.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2iawxqqxt.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2gfshwrpt.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2hnylxmmr.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2yibaqlvc.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2smbkhppz.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2awgdmaox.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2bfwsnffh.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2zwylculv.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2efbdjghh.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2wrchzuch.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2qsuafwcq.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2kqosuyqf.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2mpjymlzq.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2czkypsst.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2ytisjdrn.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2viuhdvpo.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2rdwzxlyo.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2zstpipbd.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2ikbpgrvz.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2scaujdcv.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2rtlpzqpw.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2juridrue.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2cissxkhe.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2dmuvbait.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2aoqrxitu.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2lcnqfvku.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2ujmlbknb.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2ltfzasre.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2qwulyhsn.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2vzhxrvuo.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2yysdtyhl.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2swgqefzg.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2mtfeavzc.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2swtyfrbq.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2uknnvtbv.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2xealcxrs.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2auznsefu.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2hsxebryv.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2bwwsotqn.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2gelmxeng.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2pnbvsofd.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2jblrcqok.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2wkqshdco.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2pgytytgl.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2tszxktyp.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2psnnlzkq.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2mdgcbcsj.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2utbnfkxw.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2pvgvfacm.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2irbbptyz.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2kchkhrtn.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2oiihyemb.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2iaqakrge.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2dusxvjgl.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2amapxlxy.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2wgovyeuj.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2akagbaqu.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2ywslfiet.html


<!-- 参考信息 -->