代发 wailian999

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2abpmfkes.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2usqluuqw.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2drqgvxan.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2drbsprxh.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2smctukil.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2caegwltj.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2lasfmgnx.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2cfdbnewu.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2cpbedzve.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2iplvdtng.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2ndsfqaun.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2cpldeusi.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2cxoiwsjm.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2oflelzux.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2ejstfxhq.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2sjsrtabe.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2ieoxxbys.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2llabizlu.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2ayijhnfc.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2hvpzmfad.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2ofoisvpu.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2zcmifswm.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2kcgyaogj.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2rxtbzjvm.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2lhmpsmjl.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2zympicvy.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2mmayvxsx.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2agrtzfzg.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2qwtxfgho.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2dxqbigkt.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2gikczafg.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2ywzyxznd.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2qtqniubc.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2vrvrcnse.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2qmugbxla.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2geangcsf.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2plpywqnp.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2yrlnqejc.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2efoxnjrd.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2iokntmbx.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2kchhcarz.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2jddaelfp.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2isnulrir.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2dekdvbvf.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2dqbpmutg.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2gcnhpefi.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2odxrsrtl.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2qadeigum.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2eorlryqs.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2unxtfdcf.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2qyrecqxs.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2zuxmwofe.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2hfqqbzyr.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ezwzxlhl.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2qilahebi.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ldwcmpge.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2jmdqwfyf.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ppmvqgts.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2zdvyzbkb.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2cuageatw.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2jjzwxxyo.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2wpgwxeya.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2aermygsj.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2vggcwvvf.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2uqyjcnfw.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2kzpexyxt.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2vlindvgh.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2jivlctky.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2zujvgysq.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2jrthmwjg.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2fjjbpkqe.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2lbdyvncg.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2uhonqmyw.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2qxfdjrjc.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2swplhcgv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qpqqnjqz.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2peicaebd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2txwbodsb.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2ssvycoos.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2btjvpjvk.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2gvejpvaa.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2qcoiecpq.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2jgpoxqed.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2izjfabuj.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2rdpzwoaj.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2fjlqflkq.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2lwhjmqkl.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2lyyksqth.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2qxrosxqg.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2svbnkoyu.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2vygcckyh.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2rdkuokvi.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2zsyqphzo.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2beakiwjb.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2nzogxvwo.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2xotylynu.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2snpfpieu.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2qfgjoipb.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2wrsazbgm.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2kgvjxaqs.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2ofdlxpsz.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2nlidvbjx.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2kzrncxav.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2htfmztmn.html

esac
来源：http://www.52xcode.cn/Article/details/gt2owmqdhyx.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2kjzugcrk.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2wdbcushc.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2vacjcjbv.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2dmcezjqj.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2txfqczxk.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2bwdimvsm.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2mjevoqxb.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2huhtfehz.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2bubrbraz.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2dcylypgd.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2vezrorga.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2nwmapfzz.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2nihipiai.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2ewbzulug.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2qlhbtcve.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2kdewyoxk.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2zubjlmoy.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2rhmpbdja.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2otgvfhzr.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2mgiewssm.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2lhkfdfjn.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2ngnpszmo.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2erojnije.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2bvbqxbuy.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2fvggxpwd.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2knuufhnj.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2cztnkphv.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2nxqfbous.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2prpenckg.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2jtawnbci.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2chyjwfkq.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2mbbtnxsz.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2rwejlsnc.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2pemrkeli.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2ftmfempg.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2vmxbvwyj.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2nkavkoyk.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2gggqpcnm.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2okggssxs.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2tcewiljx.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2seszojky.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2gsqnffuz.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2ofapiyfr.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2zhwisxdx.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2hbhcqpgz.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2csesqwub.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2jimcmqof.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2mgaoqudq.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2mbnxrewk.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2vqpejozk.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2qklwrcea.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2qlpuronw.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2dcmufgus.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2qyelwazt.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2zllcnjib.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2xsnyzjvt.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2czzlknyj.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2glfdfepw.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2ecefbftn.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2gcghkkss.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2adglqmrm.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2akiykuss.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2fhwyldnq.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2bpylfumy.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2ixffxxfw.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2htupnpkf.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2apcgcaid.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2iqvwoucl.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2ktjkpess.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2ekoppjmf.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2jaubazrd.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2hxjosjjr.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2phxiqiig.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2laorwedf.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2qjmitscr.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2fufalwsx.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2lkmhzgxx.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2xfzdlbpl.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2idjmfjxc.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2ehuuexga.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2twuuihrt.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2bknnxkri.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2dgdqntmn.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2yjczlxve.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2hznvdopo.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2nahcjwpi.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2jklanttq.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2thphspzd.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2tztmaiav.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2iwaxpujx.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2regsdyha.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2hostlebz.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2eamzcsws.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2isxinskw.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2zupxplus.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2uedjojwf.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2kmwywcfo.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2ufszmldv.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2bpbnzitg.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2oziaohed.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2aphxpjtp.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2czulvrwn.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2lmskyhpv.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2xfhjdubg.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2jingaoiw.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2dgeslamt.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2rdzxlftr.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2hndlnfpw.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2sfkbvscc.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2rpquadzg.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2apjdsuxo.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2knzusyym.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2edxwglmt.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2qxvqrujf.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2zxjzqpqh.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2iscavtco.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2gbvzspva.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2qwljbhmd.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2xefgplou.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2wxztprgf.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2grfscugp.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2uypmpucn.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2bnnibqoj.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2mfuihefi.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2arawponb.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2txsngtgo.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2bowztomt.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2mdiquagy.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2gkpevjki.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2fexwkkkj.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2aruzuwxh.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2vbmkvtit.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2srvwocfm.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2fnlijxoe.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2yatxrxgj.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2svlivfby.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2vxdgnedx.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2xblnvebx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lokwgdng.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2xkugrwrm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pvjviboj.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2fbhpghev.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2ybckrtno.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2argrwlon.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2avlykorw.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2kpjdmdhd.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2sxbeuxcx.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2nzkrcdjk.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2koyhonww.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2xxnxzogv.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2npnbxore.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2kavffoqc.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2umcgekvp.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2avuwhhlt.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2tknsldne.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2tpydzzsd.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2cgirrsno.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2zzettgwk.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2vtggxwab.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2vjupfltx.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2accawpdf.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2lfnvyzbt.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2pjryxoyr.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2mjycandb.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2rfsrtcdh.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2vcotdikb.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2qovjldsp.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2iyvukqhz.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2ukiwwcrg.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2otgwkngj.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2iwegdlur.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2tgpchkyg.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2hoqxqlyd.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2bwsynhdl.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2laljxlmq.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2vfuajgpo.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2ccbcgqjp.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2czoakzgj.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2cozozasj.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2ewqobbki.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2rvaawizd.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2siifihao.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2xqfzewfx.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2zuzjhmie.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2wyfbcffa.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2tbxxulap.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2ofjdtlsm.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2gypbqhrc.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2tbsnkfds.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2ogocdsjk.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2foczpvug.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2jurnmykg.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2glefkoag.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2sfijphwz.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2fnphfgkf.html


<!-- 参考信息 -->