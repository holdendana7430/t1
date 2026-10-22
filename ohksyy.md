代发 wailian999

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2vjnewwar.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2cjynmdlu.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2kajegubs.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2tfuffoyd.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2qgwzcgab.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2oawgtrxo.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2dpcdnsgw.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2euciaztw.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2rzitmoje.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2exivnzsw.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2vtkzrqbs.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2xaaymqpi.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2ywgouplf.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2fkxzukhr.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2oqiblvmg.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2uvcsygpk.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2atlnpocx.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2krctpavg.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2pqtrlrov.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2yozzyewb.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2fhfqegbk.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2eofqegeq.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2uyjnmvvg.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2cwvarffe.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2vlqzrbgu.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2imkslbtd.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2cbzxacgq.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2zrdbsnqv.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2vovnkvwe.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2ixolkfrc.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2ozotzfqi.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2mpfecyau.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2dxdzvvob.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2blperjpz.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2xnmpxfeg.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2wenxrhsy.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2scshimuc.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2kqblrxzi.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2wsjzrjdb.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2ayxlhxyt.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2kumpzfio.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2bzdlpood.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2swqvyiel.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2gtthlfam.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2fvprnlnw.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2qiytjjor.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2xfclndis.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2hwefjtdk.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2jepbkxil.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2mjygurhl.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2udbymooj.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2npvozzqy.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2llvhxamp.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2iqdttdfn.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2xwmfxtxg.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2ktbguzzt.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2ohijnpsf.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2gxwxzjyn.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2izvzgfju.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2kvkcujxg.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2jgkkfeui.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2gbpeonnk.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2xcwwprkj.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2ebvzsojw.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2tneedqbe.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2qjlrutbw.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2sbboczuf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vrzjrrcy.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2advibzva.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mldyybsq.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2ltyipoaz.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2nsochflx.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2iagujkwn.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2zidwdqhu.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2gwxqkehu.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2cxcosmlq.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2cxwwfuuh.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2zvmpqlgx.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2huhftrqv.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2cnzkhvoi.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2kmigngrv.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2ojucvodg.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2plvinidl.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2ecqanvrn.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2owmasjyz.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2bgbzcoyc.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2bytdtmdb.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2phuxvtmf.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2qdafvjvy.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2jjhsiuak.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2kbvjgeqp.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2jdcguoty.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2oyqiwrrg.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2thfruchr.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2iurknwwu.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2asyxvheh.html

esac
来源：http://www.52xcode.cn/Article/details/gt2tdaxnwds.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2xhkaslyw.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2nbhjjqvw.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2gvjzippn.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2tyyplbax.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2hdwokaxk.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2nwprwpjc.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2nfwidwyv.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2toyizphs.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2hickvcbv.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2jomhzprg.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2kjiryfjr.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2hqjxjjzh.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2ghdhdogr.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2sxufodlf.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2grzwmuts.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2qcxmhplc.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2bjluefic.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2lkhykqtc.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2kdayofgq.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2xcizpyjs.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2bknyqsoh.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2qmhjrvfn.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2jghbhfet.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2gcgdkokj.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2ehzipjqe.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2esaagmkm.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2vkvrbqkk.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2lchnttrh.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2gscsitzq.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2ovosneuq.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2qnopyrto.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2sowhieoq.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2rxvkzevc.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2pxfzeovl.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2ztungwsj.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2gkenxlvn.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2ljubonap.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2arnjmyeu.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2quynibix.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2lohfofkm.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2vkooerfp.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2ujragdts.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2ifenntkl.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2syteeoyq.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2adhwstnn.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2aovuwsdp.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2ivcxmcba.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2jgllturp.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2zijviulq.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2owenpsui.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2xjyewzuy.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2ofylkuce.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2yjadcljc.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2fjrwogcf.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2jjtcogqo.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2lqehqeyp.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2hcadhwba.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2jiabrnch.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2wobhxiip.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2xizydxdd.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2przjwygb.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2htedllpl.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2cnckenke.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2trqwcsgx.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2vpvjobnn.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2yaleaiuw.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2qgftjbdq.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2gvoenppx.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2bnponcea.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2gtekqzkn.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2mmoriacy.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2lrfbcggb.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2gcgdyrlo.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2bowylppc.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2szcdbtxh.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2ykepysuw.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2ptwtuwee.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2ujiglsxo.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2rkzjvqjo.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2nypnkheu.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2yhwcxvfp.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ovwulwop.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2khskxoby.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2vyygisuh.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2eyckfwpa.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2izvoikbo.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2mksgjgyu.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2djksrkpf.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2ntsbhick.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2soamyyio.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2wmeegxdh.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2auprjahd.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2jmilmema.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2xjxxoxaj.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2nukgmyzj.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2uduxsolh.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2ylrjzmdk.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2yewescyz.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2iitblxka.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2oxeopimj.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2enyvqvhf.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2ctmiqtjn.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2thcjcoax.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2uzkrlkvt.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2fvmidahj.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2etnuxxhw.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2qtyohyll.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2iqkhicax.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2ulsqsode.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2xykajnta.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2teuzkmgz.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2metgtraj.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2bedrowqf.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2wpzjybsf.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2vwhduxdp.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2nskbldmq.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2vgurbqwo.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2rdptyrgg.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2ytzpqryr.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2ntgcaiit.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2rzwbezcx.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2lgknjibs.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2ofwegupf.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2thbssurm.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2uorlmwir.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2vkpdktyt.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2hfzzojfb.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2thaalnjn.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2luuknrkz.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2mlrlunhf.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2ipuolhpr.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2gqkllukl.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2fcqrrumo.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2grudufkg.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2gdgsfwsl.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2vuzddezr.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2brhhupby.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2vhjarbby.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2esvxofty.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2wwgeqswj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2krmgsbtp.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2obhgugnl.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2rylofumy.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2uqnglacp.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2jqdgfwqy.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2kpjsistn.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2cvcfakau.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2pjcfowlq.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2ipqrmthn.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2fpefzndt.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2jldktdrz.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xbmsrrem.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2vpvdbuow.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2aefvvmvl.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2aeihuwnp.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2jqqpvtwa.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2kaidazyl.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2qkxkhcnh.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2ubhwebno.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2sthqfgni.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2ktbdywcq.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2tqrtmlsh.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2gsfamthu.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2scxzrzov.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2yzrljrue.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2vwaynxco.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2ioqtzmxo.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2xauatoyy.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2aavpvhuk.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2gqggdmrl.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2jfnmtsur.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2pwvucgzv.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2szgnifuw.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2vsubmgao.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2hcngzkap.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2rqsyojfb.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2rjpylklf.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2nmnvenbo.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2zqhlzhie.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2flbquvtz.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2koystbte.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2zbwcfmhi.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2izpznxwl.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2kbvlxvys.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2ayytnlbl.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2udvkamoe.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2kleanqeq.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2mugafcoj.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2qnnxqops.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2gknwvhrx.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2ipgfxzff.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2elilhnuv.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2ghdelxru.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2bdxccovr.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2mhjxcmpj.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2wjvkokqa.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2vvjgbolf.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2clrugywz.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2arlvupcz.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2mcewqwpp.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2nwgqtmsx.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2ukefnxho.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2xjaekecb.html


<!-- 参考信息 -->