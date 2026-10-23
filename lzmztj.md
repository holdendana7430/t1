代发 wailian999

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3anzzrdtp.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3yziqxvsl.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3sqenjcee.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3ulngkbky.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3qsgtrvgr.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3jlwcxltp.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3kumzejrk.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3xxchyshp.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3uvlffhyz.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3qetzvvzf.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3nmmmhuop.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3ertatwtr.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3uwapmjru.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3vikdoaki.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3xfqgyqey.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3uwieyqoo.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3nwmykisv.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3ptfvybvk.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3ecjzlbjw.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3eruggakj.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3hafnbwdr.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3dnfyoloz.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3ejkjzuql.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3eucfqknz.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3lwkccemw.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3cliuqkbu.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3tzduhzub.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3diasmyqx.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3lyiogttb.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3cnlmvkvf.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3yjikhjko.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3dmdacszs.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3mitfykch.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3zwnkwsud.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3vcurmjim.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3ikqsielb.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3mphtcbvg.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3fwzfpunh.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3ksluqgpi.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3dcxuuhsf.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3kzmqssry.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3vffogfwp.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3gzzppebz.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3ypbkooaf.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3dsglthkr.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3eqyhxofm.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3vnvydzgd.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3tgberyde.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3jonfaapp.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3rdujvpnt.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3mqzbwzfy.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3wshpqyrl.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3clmhnejj.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3qiobfwzp.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3glbxmkvl.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3otozrmxf.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3mhdcwron.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3pcgslqyc.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3wihivtwi.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3zgmoxafr.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3ahdqvmmy.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3glyhrooh.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3rcdgdcyp.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3mfexdtiy.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3lyksunmj.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3xjtvxyte.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3yjvsbova.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3dgujcjsv.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3mttymjwy.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3ueaigsmy.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3nilrvwqg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ymkpfznp.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3brgrcvhu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ypkupzlc.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3fcafxvfh.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3kxevsylc.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3tzkzrxzn.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3eaesealu.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3pxqulstu.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3ivlbverc.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3ynaqcrjv.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3dtmgwafz.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3pbrzwecm.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3ehgfnbwd.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3tutvwjnk.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3bnujwizo.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3swghwquy.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3jdrkfngq.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3wagsibkv.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3xhukfrwb.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3foceazuh.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3stnutvea.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3rlnbdicw.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3fpuunhbn.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3woxlyfdf.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3hjngxuwb.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3htgmmyjq.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3chaqzvhy.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3gvmxvzzk.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3ondvkpue.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3clowbrmm.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3xkijfnqz.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3wpjevsfx.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3pwxfuegt.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3rgmldvkg.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3daxsjkxl.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3hxcnenik.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3ghtjtjzg.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3eizpiqyh.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3wrfgwnfc.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3hrxuydcj.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3wqnzpaoa.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3mrwlmotk.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3zbfrwzgy.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3exjoshlj.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3kgdicbwi.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3svuxodod.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3waqdqvpl.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3fbqfeoih.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3tenxrvzc.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3buypiapl.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3rafbamfi.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3lpdjgvkh.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3cpyephhe.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3hrhiembk.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3hohomlhw.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3poyqdywh.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3itsnwcfv.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3dprkbklz.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3dznqomis.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3luiqyyzt.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3cgdgngxi.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3docljort.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3oapcrizy.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3tlzwkqak.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3ysnbijio.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3rghfrlgv.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3qlkaopni.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3rgajsxju.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3xjicumts.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3djrwoikg.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3kshnzequ.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3esofvkfc.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3igrpzgkr.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3rblhkgrj.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3afrjnxqt.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3pwghltnm.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3dmyjqpzd.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3mbdbazaw.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3emzhwrno.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3aiafieig.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3oqiqcqiq.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3bibopcfx.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3hguylegw.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3sehfrwha.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3riaijgwq.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3lkhcsxcb.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3jojjamwy.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3vcdcihrq.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3stavpnse.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3gzppsceg.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3ixtiwgqx.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3egeiroci.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3tjeqecen.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3iyhrhkyc.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3wjmehzon.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3otesnzdj.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3lqfxcbyi.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3pnjjbuaw.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3fbsnqmsl.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3smdjwzlu.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3ravdhedj.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3jtsmxhpk.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3hdndiglh.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3senyurkm.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3nuthuwvs.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3coterdzb.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3jbwwrzde.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3bdtdbrta.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3nbewhhnd.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3gfkqudms.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3ofukwhvh.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3mtgrntxb.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3mcxhvynn.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3njxykubg.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3ugnotfpr.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3rjcgapvh.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3hszqaljx.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3eoidyzqu.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3cqllvvls.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3rlaymffz.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3nlnxoiek.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3hsgmjvqa.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3rnleuhgr.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3gsibelif.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3jazzmktd.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3dhcyeicx.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3xihjlqbg.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3lmzeqowd.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3jzzvxonp.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3pmmdaggi.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3pbdvahko.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3ximgtrin.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3biryfjoi.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3eogfhnfp.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3skgiibuc.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3rfeszkud.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3oatshtke.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3socajvnu.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3tuvcjums.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3wuspwudn.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3nkqhusgu.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3anfwiiyn.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3qdkjzsgt.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3zozuwdse.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3wznpjugl.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3pqswisiw.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3bupjqmls.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3ddqmsazw.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3nvanhfrq.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3tpzmonto.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3swwskrmn.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3hcdcxuow.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3oemuuhjg.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3vddifdxm.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3tdgszeri.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3cmaouobv.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3iqnmxujy.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3vfagztev.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3gdbsdpwn.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3ddimqyzj.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3xwkgqrui.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3qdblgfxx.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3tbepdfvc.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3agtqcmbp.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3nblyfuak.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3jozuktfd.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3vqzqqxla.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3zmgymlqc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jzsnbkpi.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3keytiwbd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yqihefut.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3jutntlna.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3jtmhlcxt.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3oypbenvr.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3qpsvcqas.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3fdzyqhpl.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3mlonevts.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3huoswrqm.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3tnzndkeh.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3itkljekq.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3gtgnfiaf.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3fwryvfjl.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3xxbvqgpc.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3vzycdudu.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3eikhnegc.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3vygvfniq.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3qjurhhqs.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3jpjrqpou.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3cjbduiwx.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3fpxhomxd.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3dehlpwqv.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3bdpcrjvt.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3mjzlttfh.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3nkftdljo.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3nmhxxkcc.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3bzbhftrt.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3bjqmroqo.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3sqlbttij.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3acvbgzjc.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3osrffyyn.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3hdlgzvny.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3fzobupva.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3deoptxjd.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3swjxuewd.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3ukztoapr.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ambvduqk.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3nmgswhpu.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3zhlmyoip.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3qyldnzfj.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3widdibsr.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3eecmnjhw.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3rkptyxqu.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3mvcgysou.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3pqwmzbqd.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3vuzntxou.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3pasqznwj.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3lykfflev.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3dzpqwjmd.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3zkddyrzh.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3yllubtww.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3skxynpif.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3niibhdok.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3dfnwyzov.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3obwncacy.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3fvmhfpwy.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3yacmgygf.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3eudszlfc.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3spwhwrhn.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3jlzgdemu.html


<!-- 参考信息 -->