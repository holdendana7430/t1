代发 wailian999

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3dllrkvwy.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3aglshxlu.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3zuzuizlb.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3evzciuhc.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3rmgwuqnm.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3mknuegfi.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3wzgefqgk.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3ujjdphzt.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3ojexdlar.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3hedevnih.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3vrowrgga.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3zwlhqkrq.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3cnzcxzyt.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3jmovftgy.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3sjqdnhgk.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3egoqburd.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3udqvohiy.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3abdmkumx.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3gkuchenv.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3movumodu.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3yvcaqffw.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3hfjvrqju.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3bevfxtqm.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3fnmjkpro.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3shwgdouj.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3uuskyduq.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3amuoxrtu.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3zbgickft.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3ygcsiyub.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3egfjyovj.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3mqqphwhg.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3luioyjcz.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3pjswcorb.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3oerufljw.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3uelzthwr.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3zxqwcqzw.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3fcircyov.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3oummndpr.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3nredqpoy.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3owgnifuu.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3keohilaw.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3exsitpbd.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3lurwfdcf.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3braafzfe.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3konzjniv.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3tlmwzgkx.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3hygdosvj.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3sdatgwyu.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3uniexqoc.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3fonsynyk.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3izmeyvcl.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3gjhlzwwr.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3yepdijqt.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3nvbvjamr.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3akkifqjs.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3kowxcyhm.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3mudebtcx.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3jpzqohiw.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3ghfuqtll.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3ppzajtgp.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3jiolents.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3sbewracc.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3ndawwhyz.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3mjmgydvj.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3ifbofvvh.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3hjbqfteq.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3aommkbzg.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3xfsjjsgw.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3ozwwsfuw.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3plnmofly.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3gxvntdqb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cdruycoi.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3cightpou.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wwojompt.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3mctphxfa.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3uwxxdijc.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3bvjbbvpz.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3stwvmdnb.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3ggphufvz.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3piibunxu.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3kcxtdwrc.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3qyiqrqmz.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3kywwalel.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3qcsykcke.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3mqlzzdnn.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3qsawnnfq.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3tvuiybbi.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3ldtfwxnz.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3grylqhik.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3gfppalvl.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3yxzagfsi.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3yjsdpyty.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3flchnqyq.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3ajpbhwrp.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3vchsfiye.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3gjjejwgq.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3ecpqlvvq.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3ayotnijz.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3kbyrzmtw.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3ifervsde.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3hjbvgvnh.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3ocvtcumk.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3dcmwjmsr.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3ooeurnkk.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3xylvfybf.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3uxnkrksb.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3fbbisqwu.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3ootluaej.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3sebjpwzu.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3jcvdqirs.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3lvufhlvf.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3zgnjqbmn.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3jxgeuymp.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3vwkoqupd.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3syusapgh.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3soiatgpw.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3ivnkljam.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3yocbjugf.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3dbqjqjej.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3fcksfmew.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3fpfvakfv.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3spxnzamj.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3aihyvdkh.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3xqwsijlg.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3ksjiietm.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3qmrlgrbx.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3qzcaoohu.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3ohztsbgf.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3ulmbnefy.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3rfseynbt.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3fmjatxva.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3xwujkorx.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3frpnkvln.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3pmesfjph.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3aombpllu.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3zwzfdlxk.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3cvoqiwuj.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3xitwrewi.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3gwoiphom.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3duvgjwzz.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3jqykpyeg.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3xrvzuqrl.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3qmjvzpom.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3zljxmzrj.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3ivlfkysx.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3iuedzvcf.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3mikejsfa.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3udefyguz.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3stumfaqn.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3sujfeptl.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3gyhndfdk.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3bkyuuhgo.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3ajcwptve.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3fwishiis.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3dsfzxses.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3scwghmmw.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3wtgpuggn.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3swnhfdbx.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3kzyixvci.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3nvofqrsc.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3jwoksdcy.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3cwkmsjqg.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3xkzzjdyo.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3mxkhhqnt.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3gmzzkvxw.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3rgldpprj.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3etltfhlw.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3qoxegyxm.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3oxyphiay.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3kpjslobo.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3lwaqugrj.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3hqtmvcye.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3vvdwirws.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3mhupjuqz.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3nrrqkqnu.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3qkewgdwb.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3cwfoartm.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3jpeewtkr.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3nwlqabbn.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3ccvglxpo.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3kfetauwo.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3wigljdmr.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ouvkhakv.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3uccldwtr.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3fsxliuek.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3umzjkfua.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3bylbcsws.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3zidwwgqn.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3useulblg.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3opnlpnqm.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3satjgmoe.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3yufuymes.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3cgdqxjwg.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3bonazyvw.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3ovjdfoon.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3plpbloab.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3gffmrmym.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3bawhiiug.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3zgjjjsrr.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3wslwpdvu.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3uigzkegb.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3wxhycmpq.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3gcmxdskk.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3pkhpfjha.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3usdgphig.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3wuijobjc.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3wyfkcaff.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3fzvarcfx.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3qgmtzqmx.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3pmgzinkf.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3hevfessl.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3dwmufrxm.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3xxcwcwcu.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3tmgzezfi.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3zifbmstz.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3mqscjytg.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3nlbimdeq.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3ikcdztry.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3xvyueaau.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3znnjnwxi.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3xwcpgher.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3igzhtczu.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3msercpgd.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3padeviwk.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3kkkukgia.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3lefcbtfk.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3iklksnrm.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3janzvzch.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3dxdwmndu.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3suxlfbad.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3ofomgnqk.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3iajhyaab.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3zxodluzw.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3afkuuwqh.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3dfpegiar.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3stuhkhwl.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3mcyuenna.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3hcdtepwi.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3sllhlseg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qqrzulrd.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3bmpoemdc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qtpkcivr.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3tnelfzsj.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3odenucqg.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3mfsxppdg.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3diijbjly.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3imgpwiuu.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3cxrezuvl.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3cnyzhlon.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3jroczidd.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3xkmvlyxj.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3qezyfmii.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3pkocqxyj.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3yyrsfugn.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3bzxeabat.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3uovuroql.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3yixeljng.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3butrfowh.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3oionydub.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3gxbudaef.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3epxompvs.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3woceifat.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3nguunzzj.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3rvwqlztx.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3vfvypzeu.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3lmmdmtin.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3hkjctazz.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3ldnqehpg.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3gqmreldi.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3exzuezvd.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3fzcvluls.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3apvtlgch.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3ftleqrfa.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3zibudmqh.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3xbwrdjtn.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3sknwscxs.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3bfidkfql.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3stxxigbw.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3clhqmqpf.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3qcxnhlah.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3eaulctok.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3mmbvfwro.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3nhgjjbwq.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3vgyitkzk.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3tbszbnhi.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3yrtnavsh.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3bzmnhaie.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3nwrleocw.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3tutfhaik.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3wztpdiqb.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3ooqodigh.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3lttfilpt.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3ndplsjhs.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3qfwwwosa.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3kzkuweux.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3taoxaoee.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3udzwacmp.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3mqulspjl.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3tnkhabvc.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3krdyxppo.html


<!-- 参考信息 -->