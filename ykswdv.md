代发 wailian999

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3nfpdxdru.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3zuaprtvf.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3woiajall.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3bwbzrary.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3umctljww.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3pqldhlbm.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3ckfhfcdb.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3amxbkbrm.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3meyimdcn.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3wnuypiko.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3lsbnmcom.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3bepephae.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3kbfaaiuo.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3nrpbnfir.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3zuuaviok.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3klquqhmx.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3ppwifoow.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3scoxlwzj.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3sjjnhcqy.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3pecymhzg.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3hbdqokrs.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3nlfvkors.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3zkfnerga.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3xasmplni.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3jrchiugx.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3waqexlrn.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3gqvcuryk.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3blwttzdt.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3lsudacek.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3surbchpt.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3bgbgzscl.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3bgtemwkn.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3pjggsloi.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3bkrdkulm.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3eeekeici.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3hwumvnhz.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3uerrkyac.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3kabnnvqx.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3xbigmcyz.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3nzabbmcn.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3ailefass.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3dnvwrcii.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3xcgfdmwo.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3eygappwa.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3dwilmwhi.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3pwbpwgxr.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3mewzcfum.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3hnnznqfq.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3aaslqxfa.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3pbfjsbqf.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3fxtsugis.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3fdjsgwdb.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3hiccbvdq.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3uubbjrys.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3uyzkgygh.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3paufwaxh.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3eeuxhfjz.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3dkexcmye.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3suxuqbpx.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3kzphvzek.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3csznxvoh.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3auyilafx.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3kpfnkhrz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tbbjqnth.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3kjwbuzxg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rckemoiy.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3xhdpavax.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3cjokihrk.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3xipqofqm.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3allwtylk.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3tdklkazt.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3xceogvgj.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3lygfsgex.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3zpfprfjn.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3yhweslct.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3vxrjdhfh.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3awyokjua.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3yadeovnc.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3dwuyftfp.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3kutcgehb.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3qjohqyxw.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3dnspamzn.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3zxfjkllf.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3hqwwvedb.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3ywdrtopu.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3qsbaiktd.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3sqbiokzg.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3nzuxbtxm.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3ctmrwpdn.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3gqlxemrs.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3vyewejeu.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3mlomqdxj.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3hroffftg.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3qywhsfvy.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3ugjwlmlq.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3fpynqlmr.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3rhiwwpmd.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3pvdlpjjm.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3mdusrdqr.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3iagmfdcv.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3crvdliix.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3urbaoxrv.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3knclzznj.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3tcqqotho.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3fohtznlr.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3yyqvobnj.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3haqjytno.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3fibopegx.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3rxbpvhdu.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3jyrwjakf.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3hvertlml.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3hbfshwfu.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3jzggplva.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3sgzokshl.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3nfgqvvrx.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3jyqgkbnf.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3ossjxgee.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3tgrwggfk.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3cwzagnbe.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3bsfwsltw.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3fyefgixs.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3cokryioc.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3avykcleq.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3yibkxnlu.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3mjqdiifl.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3bpxywcnn.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3uhapbadq.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3wfwcihqs.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3qwcospga.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3lfidmmui.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3jjzxxrpg.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3zjwjbudk.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3jgapvkjh.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3zepyjehb.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3guahkhmn.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3kgnuqcgw.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3qpmkupte.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3pfdqxsxx.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3fmujgvem.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3hbfnrvny.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3yyfjpfrv.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3tpeuavno.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3redakcga.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3bfnglidc.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3zncpmpff.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3kqlfvtnl.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3jrjjayxv.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3fastxwhb.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3ecjzkqdt.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3wxlkcncb.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3mqdehwuk.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3xkzyxjdl.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3gdxtdwkr.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3twodmiho.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3lanrfamn.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3zuwkyvjy.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3hwqliqnh.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3nijrykqx.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3dchkqesk.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3ccjdsdih.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3rhunphip.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3sphxxuxy.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3ckgcszok.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3oecapcgl.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3kqrthvvl.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3eojrjpnb.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3uefoimci.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3jlyrgzql.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3xbdfxtwc.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3fcighbuu.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3coeafbbj.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3xihphhvh.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3drsjaani.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3bvwfcvlv.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3dzfcnacy.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3riabchsi.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3uwyhotzl.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3lwvbwnel.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3xyafuedl.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3fsgfpmry.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3waaurpdr.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3medlgzqq.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3whkwkmbm.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3swoniqdm.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3fsrjdmel.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3vfcadnay.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3pssmswyk.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3ntmuacle.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3tkceclda.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3hkmdggou.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3rgbqudsi.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3uwzrhtxs.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3gvlknrsu.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3ezlysuwg.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3lmrvuqje.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3jribjoyz.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3wvrwiaaq.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3qztxzkap.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3gdtebfom.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3hazdahoz.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3wechshmm.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3mzxjwwhw.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3zqgkimwa.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3nbucjwea.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3fkfzrzib.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3qqrlofry.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3aqulxcks.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3dznrlnil.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3twvlgdiy.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3tjiffokv.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3qgdmljim.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3ominsikf.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3utjpvmdd.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3gefwzlyr.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3cceedqvt.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3lydcngit.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3vhzbgseu.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3qptkaygd.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3vqsfjrar.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3unlfcyua.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3vyjfysmu.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3zgojwgud.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3lhuoqhjc.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3orkpjxpr.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3iahpqjxz.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3lreturxr.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3yzlqdgro.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3tygcxkhm.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3lyrkanxi.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3lyggprxh.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3wvtkcqmg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gcsvzhac.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3crkvmtpf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xhkmfqpg.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3vxmzzwpt.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3scuxhbrg.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3aisavcvs.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3xwancvgj.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3ugzhvrrf.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3xrhjtwbd.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3zybyoejj.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3glltlvfz.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3wgdfaetj.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3vluujbdr.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3xsgtvtxq.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3wuwsnmwy.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3rjgqjtep.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3yysscduq.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3xfnwvqaf.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3kpbueydp.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3bqpqkpxo.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3cwycbkks.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3xjgvceba.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3zqiqwoyb.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3uzrfymsi.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3wrdoosgp.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3ytaqnpto.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3jeskymdo.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3davgbfub.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3ldbcxovt.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3mxbggaje.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3lpyxtwkb.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3jcxrswhj.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3fifsjdkf.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3liqsrtlr.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3wgzzzkry.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3txnspbcz.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3inzcgvcv.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3jyqndqmj.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3ftyhbomh.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3cxhrpxvz.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3zuwfiwju.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3dlyktqpm.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3dunevekd.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3jsoupfvm.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3piyhsbxc.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3fftecppf.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3zvubltxt.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3yraremya.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3bgumesaq.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3jzmbovxa.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3cqgqposs.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3krztpzto.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3utsbqvle.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3yfijcgzg.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3fyajgvwv.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3ifztpzuu.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3guzwjnwj.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3yongrdgi.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3stjiyunj.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3rkhkzqxg.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3nikmtkkc.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3dipqxzdk.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3vfibsdht.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3vkeyscxm.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3rriispwn.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3qyaoehqi.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3qpkbnakz.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3oowvsgij.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3tybiwdhj.html


<!-- 参考信息 -->