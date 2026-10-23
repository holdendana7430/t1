代发 wailian999

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3plwcbbin.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3gylcwydd.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3nmhyhyyq.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3paurlqdp.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3bllnzkvb.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3snrjpicr.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3yxbtnygp.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3gtzxjczt.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3pmhotxli.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3imcjzavk.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3ztiowrxr.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3rldsyqiq.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3bcuxtjlw.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3dyvuriry.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3vezwhzxz.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3pffapvgq.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3zcgfpetf.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3tvsqmrsq.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3rrsqavdw.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3bnpgcczk.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3xfczxusm.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3dpoxkffa.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3xpffakov.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3flqkjyvc.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3sgyrsles.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3fljvvqbc.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3iakmbcwz.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3egqrpcon.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3yzuastyx.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3kjzdnpyp.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3klzzwslz.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3hwxmeokr.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3xvoaylpb.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3diruutsx.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3bkiuebpb.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3hzzvazen.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3vpldjdpr.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3qypiqems.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3bakmomao.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3zovessth.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3lpmmfvxi.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3dcoejbxp.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3hhqcavwm.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3asdolgyf.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3czyfhxrr.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3tzhihlbk.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3kcgxreoi.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3ikrbjyon.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3noithous.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3aqxqjjzr.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3iagocdtj.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3fewifhzi.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3cbyxlomt.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3kdsyydeq.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3bvdrguje.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3nsrpcnmw.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3foixnckw.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3misfynja.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3kmrownck.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3ujditmmo.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3xhmbdknp.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3zsrxsbvx.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3bvzhbban.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3dkjhbnlz.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3qkitrirl.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3stfzpeae.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3zgkjfnme.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3vgawzjjm.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3zondwgdx.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3karibagq.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3uphyuunu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yzibqvki.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3pntamisu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dsufbgis.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3ychlycji.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3bklpusgm.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3hzvntkbo.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3wdhqcxny.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3nvovrkjl.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3birpiiud.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3ozhenlmu.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3kbutmeon.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3tnlplkrq.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3pghqslfv.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3inqsajvp.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3kcxlmzof.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3phwfsvtm.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3fqtvkzns.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3rvveqfsd.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3sxxgkjxu.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3pehnmgin.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3nwewaahi.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3stcvlrrb.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3bnttbsxa.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3kpbozfqj.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3gorvlqvz.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3wdofslsc.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3wwldoccq.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3tcqinjxc.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3tmbuudsn.html

esac
来源：http://www.52xcode.cn/Article/details/gt3qzaaeiwr.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3bdqndenc.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3rlwcsxbf.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3wgzemhdu.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3hbjsbnar.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3ybuvmypg.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3asyucfoe.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3ubbuvaws.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3sikrzuif.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3rsqndamq.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3tjrtasxk.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3vrpyusdh.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3sjjuovvs.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3ckbxuwsy.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3ebtlrrjy.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3edmlnono.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3jlgwspkw.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3xdtpfmzt.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3kpaeameg.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3khyhxsik.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3ctbfrgit.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3oqhfspyf.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3vjsrntvm.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3fcucslex.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3gfdbuifp.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3ygbcrgif.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3fhqsxqlc.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3nftyawod.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3kmojljgq.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3vmbqxatf.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3zqsjblnb.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3rjlzmrht.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3vhjpydez.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3pkhzhqth.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3kdfejbiu.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3gjgjkcfm.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3uhfatukk.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3ziewkbdn.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3colynaus.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3muasdcei.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3mgrylwzx.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3ogtlacpl.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3ikzbqaya.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3lzpjlngg.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3jvkieuhz.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3krctgzrd.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3gjpkkgqh.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3bzjdfckj.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3beaqefsm.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3vntsabxt.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3ehvtkasw.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3lyzmqmek.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3djxqzgvw.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3thpopjxf.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3puwbfeaf.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3cibwmdkg.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3lkgozkme.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3ownrhcec.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3burjtqdx.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3qwnyhwxp.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3zbxyytes.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3ggsacpqi.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3zwrzhktr.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3ccwvoigg.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3umvtqkrk.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3lrhhbsxf.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3yznlqgbn.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3uizecywz.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3llorxcxw.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3ibbnbllv.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3yklxghfi.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3xmeuwxru.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3kfvidpcc.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3pkcldttp.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ijnawahm.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3ddtvyxuk.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3kflyazkb.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3orgjzntl.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3vjtrnfou.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3qxlxycst.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3moafvcku.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3lmephugh.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3mfdmrrvh.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3vwuzbemr.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3ifqygpfv.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3apeciiff.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3vxgtzvfi.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3ysawexdz.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3ujglaydv.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3gtcyilpg.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3rriubjmr.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3bmwdrbdg.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3lhffkzhw.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3wzodxmem.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3nhpbzerg.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3dcizqlek.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3xtlqzxep.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3grzzzfvh.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3rgjlszie.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3caicmpmn.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3eykzkhgr.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3ghiwkpeh.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3dmcnrczn.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3yjbrwkhs.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3frpzuoqm.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3lhicnhca.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3atxictcd.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3sxklbaty.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3ijwridrc.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3ibsahpnx.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3kklgdtrg.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3kwltsakq.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3kclgvrcu.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3uxcdigic.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3iuniczkm.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3jlapsbwv.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3feviagou.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3umxlmawm.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3apgvswcr.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3krvtuudk.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3buemeffs.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3rkyyqqer.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3rbnztgxj.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3mfuixoqv.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3cjoeyoxj.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3hisbonce.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3tloknugi.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3gfzcurwz.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3bltrxvoh.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3jcthpumn.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3wiivtzrl.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3xxntxzqx.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3awsjiooe.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3pcglcoha.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3dsvjgjew.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3wsffvnes.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3jihtzxll.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3jlzijfjf.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3gpawnqhi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3feqktivy.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3tncmjwxg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xoqlwsmz.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ndmohnwi.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3gehgrijb.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3aqeecukb.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3irgjltdg.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3bbhvugjg.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3yumyhmyr.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3zhbtynia.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3jkfwubyi.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3bagphgpe.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3oeaaytqo.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3mkiczehz.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3lfvxrbpj.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3fzdpyiii.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3vziowdkz.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3axyzyztw.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3phmhnioi.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3pxniaujg.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3dwnmikrh.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3dcmwoxht.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3qusbdcls.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3sulnvgtx.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3wysykuiy.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3nyjdbjpj.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3zpxurkbg.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3ghvawiez.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3zttzgnwv.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3ezzwibmw.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3blivpeui.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3xiozqoqp.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3vmbiywvq.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3gormlkbw.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3szqabokc.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3fqethacd.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3hhoukyxf.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3cadlrbbp.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3hjhkydfm.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3vqrjwjrj.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3luyrimhs.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3gpyuqkry.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3aftvpnab.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3vkemmauk.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3wrnpdxia.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3feqpvror.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3kslcegvq.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3ghnkmrpr.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3qmmjvyqd.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3njplwmta.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3mqsmjlza.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3ixmdqjns.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3ltmnzeel.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3gzjpuglu.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3npgztnat.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3odxlnote.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3olovrteg.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3jkxliqlq.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3zbtjsagb.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3kjvxxgwd.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3buxltkxc.html


<!-- 参考信息 -->