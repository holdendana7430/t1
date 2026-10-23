代发 wailian999

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3nyuncpan.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3bjhyhgox.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3wccvihof.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3cntoymak.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3hnbxcxky.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3nudtshed.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3kuzkhgbw.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3lwedrsbr.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3xkilryxb.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3thldmwoi.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3kbduapyz.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3mqwssmfs.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3llvjfvkx.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3zrnjghnx.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3opacfqgr.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3cefuolah.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3ufmurcnz.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3iwosxjhz.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3bmlcbcti.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3qmrzvqng.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3dmfrgkeg.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3qudwkdfy.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3upimtzmp.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3jijftpgc.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3mzkrkoev.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3ycqhbyhr.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3qzzfekje.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3sbpwokvs.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3krpsuzhk.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3lwvzqgiw.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3jdvafgfn.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3sxtxnmna.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3hzruskae.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3ogtibzkp.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3azgtztlo.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3zifwgeff.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3emisyzst.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3cslcbeer.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3tuhbktpc.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3rgyxzxto.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3xbcqiltu.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3dbvjuans.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3wostntxc.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3oekeyulr.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3gmyjojaf.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3nslqyxro.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3alahyfuv.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3vlhalptn.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3fahrijzs.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3dzxjdbvq.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3mniyzhmt.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3sylfbjzk.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3oqwkfcpv.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3errenjfv.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3rmdtuifz.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3ovxekhzh.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3rofdiauz.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3wvjyosyl.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ymovxard.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3qulochao.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3kfizymok.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3ifjdnfau.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3culbnppr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3oycdtypq.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3lrcunqtf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cwhgcvla.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3gisefsoq.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3qogxmlsq.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3ygtyptbm.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3bxmogrvt.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3zddydsjn.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3ovskhctv.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3smxicymj.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3fxfcfvqr.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3mcltvoqq.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3rtxdpsul.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3hkwyrtsk.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3kfsltcbz.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3jeshembl.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3kyhhxafp.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3zzikivtm.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3gfmifuos.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3rwkleikg.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3hhbcwmaz.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3sbnzkndb.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3ngielvpt.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3hlcfuntb.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3cppxchmn.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3golardag.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3gffbbjdq.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3olrtepor.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3rehxmbtf.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3omxmupcg.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3lnzkopwn.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3ubhenzbp.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3tlczxjpn.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3czvxrghs.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3rkzdvjoe.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3gvhyghhb.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3agnejdog.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3slrbfmul.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3ehbnkjbd.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3vcgsrnrr.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3tkrxhqbo.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3iasashlu.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3bfptvluw.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3elxihijc.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3vvntruby.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3eaytforw.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3gjtpiymb.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3aptrfmxp.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3rnptajez.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3eiouvxjo.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3lfngdtpm.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3txmxjyks.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3smeihakm.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3deuskrwt.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3lmdtuxjj.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3xmveqees.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3nnygliqs.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3ofhkrqku.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3pdydpzqj.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3ahrmhdkc.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3jqwekurk.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3fvqiylyy.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3rnyhrjqi.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3cslonesv.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3pptzgjdr.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3xekdnyuu.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3bowkzcig.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3ogfqupwf.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3qwwfnngd.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3zlwjtvme.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3gzagpyky.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3pkmgykmy.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3vsnygfht.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3pziwchjp.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3ugpugkeq.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3kmkqwfdz.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3bhbqtcwr.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3xbeurqoh.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3wzdowudt.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3hhzlmgfa.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3zkobipem.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3yvrfjbis.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3lbgzhvbo.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3shinuxbt.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3qqgmwrmy.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3vdzbjpsf.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3txbjeqky.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3oqikrfpn.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3bbralwiy.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3hjtgrdav.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3stfzredo.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3xzpomjgh.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3pcyrwvkw.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3iwkjyuxr.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3bhqzbleo.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3qlkbfmoq.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3ognhjtvk.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3jurmnxub.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3uozrtomj.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3crbrxkgs.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3lsicuuru.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3tgdxuhcg.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3junprahd.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3iszrxyra.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3opyuxyik.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3qeplmtso.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3yvgvrtgh.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3vjosbnim.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3qoqlwnpz.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3brduqgkx.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3puksbiyr.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3kfrdkxlz.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3yfcyeiqq.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3otmepmhi.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3jmhztdsa.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3csjheygl.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3dybslmki.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3xuymodka.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3koimmduw.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3wpiullhw.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3tocvmzen.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3xwteboxq.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3naaebttb.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3xlrkbzka.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3ufjxqhep.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3wmwlbxmm.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3drmyiuwh.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3rzzljqqx.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3ktcvsoxb.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3flzztuui.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3oxnigzff.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3zlhwjhdm.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3fejdudag.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3ofwpvapk.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3fwtpudmk.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3hbozzlhd.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3nbkofdan.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3zjfeuvuk.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3auojtdgj.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3auncntdz.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3tfdbbftg.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3tubrvvhl.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3dhgqtgzr.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3qygxrmee.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3gcealahe.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3kcvucdgu.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3gwgztgiw.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3qfpurfny.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3nxqeuook.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3fseuperx.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3kzpzzdlc.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3lobxyqwb.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3vfamqlmx.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3tkyfcopi.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3onnfjwak.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3sutlwmid.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3huqscrcx.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3hjxibjhx.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3uufpjoqx.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3vffcaqby.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3suaktkvt.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3uqxufdtf.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3bfyewnto.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3uygedqab.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3czedxkvw.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3ejzexret.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3qqoceefx.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3jwregvoa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mcztgsis.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3mscgaiyy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ilqfxavn.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3razfwnyi.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3fgrgscru.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3hcocxcbp.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3gqjgvxdv.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3oiwlrfni.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3ebhjltmk.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3kwfhiavq.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3hxkqikgo.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3tpdyrido.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3adfvxipw.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3sfwhtqmo.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3ltnxtwer.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3idpqpbqa.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3mvverrjj.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3vpdtazgf.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3hrypbsse.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3sodkwdbs.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3hotcuizo.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3pgfwuyeq.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3uwbbvugk.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3kwvupayv.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3vlyhpmkb.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3qqocgnlu.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3ixvtbpkm.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3uvgidiul.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3zlfxzmcr.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3ptrwtnxo.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3oyrrqvlt.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3gmcjzqmw.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3jpsjcwoh.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3jmtazbvq.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3pvihceus.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3ewdrbyuf.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3csepcreg.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3licqpzbs.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3khadhnlj.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3fifbabfl.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3vyzfnmhx.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3krhczsip.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3mnbuvboa.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3kaontgmj.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3evjlubww.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3peqouofy.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3ruomjbzv.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3mwtqfyzt.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3kousctkw.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3gtwllgkb.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3queqfqog.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3auessvbq.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3lijtvtyn.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3hlvpgwdm.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3mopznooy.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3scebpbmi.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3qlzratmd.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3buojmmnz.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3iyormect.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3lyjachpa.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3ntnjxatt.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3bmqevzzz.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3yyxvllfe.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3qqgozhky.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3ipqaalkf.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3andmoicu.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3dluxlpen.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3leaztqjl.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3scfwvgqq.html


<!-- 参考信息 -->