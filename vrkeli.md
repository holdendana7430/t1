代发 wailian999

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3cxhkwkcu.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3xebnegnm.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3hhvbveua.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3amvfiecq.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3ihqchqfy.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3ukjnscmo.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3zzqxenxs.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3nrwigcwz.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3xtsxrroc.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3bkibiebw.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3ocjvpsqi.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3muofrimx.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3dazxttyf.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3nundvqkb.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3txdctjiv.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3zxbruiiv.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3jfemdokx.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3qhshwxux.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3wtbvkhfb.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3pdlifsiu.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3charsuef.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3gceuqxxn.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3itoxdtqe.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3vtztqgyl.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3lymxbrdj.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3cktipcnc.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3bosbcfeq.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3vuqfshff.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3iyyvwmvo.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3mmuguztm.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3wvygqikz.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3juteygxq.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3jybjmqsc.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3teugnzux.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3duitdvxv.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3slhrhsiz.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3djpisiwf.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3jyhkxiyi.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3slzsloxz.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3dovbgmek.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3thgylykn.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3fytyabkj.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3wrwidlmo.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3lfknwufd.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3jxinbvhc.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3clehndcn.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3zxnopnyh.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3cusapuga.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3fdujklqq.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3wgpxrhlh.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3czxezacv.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3jmogebzb.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3rifpdczz.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3bwzatisy.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3hrzxwxje.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3ujofqucj.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3djjdvmbo.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3hfjuwwkj.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3dnjqhgin.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3wsnauxnb.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3xyjduecl.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3peaczmuv.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3zkgqgppd.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3fonjiflq.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3dnmnhmyg.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3ctoxwjgp.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3pftmrfkb.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3cctwinhz.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3fqyeggon.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3sylvvqsh.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3pzckxucb.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3neoscfry.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3pyxjubqm.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3zlokndzw.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3zvrkdfss.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3fqidmtve.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3catauhbf.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3tzaomadv.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3rfxkeyvm.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3ghbgpgks.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3rwlsbtfs.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3xsfvhwzo.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3gjutijdk.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3kmxrbhqy.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3dyhqqjni.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3iqpykbjn.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3vcedqrbh.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3grlugxmu.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3jpbzvpkp.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3cdfoyunk.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3qafygxba.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ckiiposp.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3mbxdlxow.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vxrucecz.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3coqbjebi.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3zlptgjrg.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3ysmzhhri.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3sbcpphfq.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3denbxybw.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3evyqvrvj.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3aktzgbnm.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3khplgsrz.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3srazctjp.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3uwnnpqco.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3ludmklup.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3ffmzvxum.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3xgyfnbwo.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3xrzhfukz.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3gvzmzrcq.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3zzcnxbbe.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3qeiohpjr.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3xanwtuxx.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3jthtpmqs.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3eaxjhkrk.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3sbgxnynt.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3xzupyshg.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3zrlicdos.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3lveiethf.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3igejecmp.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3dlhwvkcq.html

esac
来源：http://www.52xcode.cn/Article/details/gt3iddctvsa.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3wqkelusb.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3bydkjuwm.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3xlbpulyh.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3hojsboia.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3mdmeoyra.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3qcqybjsi.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3npzejtol.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3vvaqcwtd.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3qgjfaknv.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3vuvzqnsa.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3pwnskoke.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3vgessumg.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3wchzccjj.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3ylevjpqh.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3qkipwfvj.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3mbcrzrjz.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3zurtbnyu.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3thevdnzz.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3updgwuox.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3btfclile.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3zgyentyl.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3ajutcgwb.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3ddbbssop.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3attnokjc.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3aigglaos.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3uetedymz.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3ohnfmrla.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3yytpvvbn.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3rfsydrgd.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3fqmctuyz.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3ofyxrqar.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3mtjrpvce.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3ybjicurl.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3mxphiqht.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3vlzdozaa.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3ywaaxfsh.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3xkjvveal.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3thuiotql.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3cfdazjpi.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3ehbocotp.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3avddjnyy.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3gvoawugy.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3ajdpidlf.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3mdclrdsa.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3zdynsshl.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3bogxpxpl.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3wofxffjk.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3tzxjdhgn.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3ecggnmqy.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3yhquepet.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3rxnjiahz.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3lllkwliz.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3ftrhejma.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3pnctyouq.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3gtqfeyoc.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3hyhscigm.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3ekktnqtm.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3ywduyrgc.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3rypvnyjq.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3qmhudfkw.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3pnxqejvc.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3iihkqygn.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3trnwdumb.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3xrnwlzot.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3qxlfyjpt.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3gdezhvpk.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3xyblcvev.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3dlvstcjs.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3zyzhbzjz.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3jcculldq.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3nmnkqwmy.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3vhgtueou.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3izoqvwvq.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3uueeslky.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3vmwrpvsa.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3xcoxwyrr.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3wgimrmdp.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3xamqucit.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3czlosjsc.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3vmgcbvvj.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3jvtuwmzu.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3moktgcpw.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3szyjwhvv.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3izeiqztv.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3xwspwkow.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3owxyhean.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3nfovynuc.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3rixxgrec.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3xjsmeano.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3qylpuofo.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3vitfknoq.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3znspfbcs.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3zvjtgubt.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3liavdtpw.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3sevaxagx.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3cngswlyt.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3jsvxmvws.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3nuwqcphl.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3yokhzxox.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3bintfknw.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3pbbhdpmi.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3pdvawrou.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3euiavooa.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3ssttqcvz.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3kmattjcy.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3zwekrhuf.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3vlbiimoy.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3sigipjcr.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3xdxuhqgw.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3rttwageg.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3tuofvwof.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3bmrszjaw.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3atxghlni.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3zejiomua.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3irtzwzkf.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3wveifeps.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3tsxpkaqa.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3iwnvlfkw.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3oqrbogbs.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3gmlgbxxv.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3ixdspgsm.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3hdvguzvj.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3cotuxacg.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3ehtkdltv.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3plamkhwi.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3wkoolacc.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3zkopetok.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3ncvdtpze.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3puzzzzbo.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3twdmnjnt.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3lgqjoyji.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3dwrsvtjf.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3fwwiglpr.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3sgitpnmx.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3tdlxrqti.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3efosqtzn.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3opdibdmb.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3cuclyxwz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wmfnoauz.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3utbzxznb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yyprslyf.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3dfgskvtj.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3qsrcjfyd.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3kcmlrjvp.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3pyettogg.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3espiwrae.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3zpovkpkc.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3purjtzdh.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3jmhuejlu.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3eisvttms.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3sctryxhr.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3joctzwrw.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3vpncxzgl.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3lymhmzyg.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3znrbnire.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3lmnjcqcc.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3nlnlywha.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3vpkohcyf.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3mthurdtx.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3lhylwaiy.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3erwphpvb.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3makfwnrx.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3eqbgxasj.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3axkufojx.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3hahsjrsm.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3izcttmgp.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3epqyibrw.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3zydlhaxt.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3fawdxcso.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3demdfkav.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3tgxseasn.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3jtmpmbpd.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3icbtperx.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3skanrchj.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3azczqovi.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3uomjxaao.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3omjfnrpj.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3svkkxivl.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3pquuawhz.html


<!-- 参考信息 -->