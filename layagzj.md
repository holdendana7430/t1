代发 wailian999

[Q65] 回滚事务
来源：http://www.share.fanxiaobao.xyz/Article/details/gaejifbeq.sHtML

ROLLBACK;
来源：http://blog.fanxiaobao.xyz/Article/details/gkccsedub.sHtML

[Q66] 行锁查询
来源：http://wap.fanxiaobao.xyz/Article/details/gaizlttut.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://m.share.fanxiaobao.xyz/Article/details/gsvuoylek.sHtML

[Q67] 设置隔离级别
来源：http://blog.fanxiaobao.xyz/Article/details/grbvqmeks.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.fanxiaobao.xyz/Article/details/gbenffeha.sHtML

[Q68] 保存点
来源：http://www.share.fanxiaobao.xyz/Article/details/gfpwnoxvg.sHtML

SAVEPOINT sp1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gjqhqgdlt.sHtML

ROLLBACK TO sp1;
来源：http://wap.fanxiaobao.xyz/Article/details/gcsjzfnsi.sHtML

[Q69] 查看执行计划
来源：http://m.share.fanxiaobao.xyz/Article/details/ggtnpnqtz.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.fanxiaobao.xyz/Article/details/gdafapaoj.sHtML

[Q70] 更新统计信息
来源：http://baike.fanxiaobao.xyz/Article/details/gcoritato.sHtML

ANALYZE TABLE users;
来源：http://wap.fanxiaobao.xyz/Article/details/ggweaorbc.sHtML

[Q71] 查看建表语句
来源：http://www.share.fanxiaobao.xyz/Article/details/gayotuxjp.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbtykrlrh.sHtML

[Q72] 查看索引
来源：http://read.share.fanxiaobao.xyz/Article/details/grvxsxfil.sHtML

SHOW INDEX FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gxbruhdtd.sHtML

[Q73] 查看表状态
来源：http://3g.fanxiaobao.xyz/Article/details/glsgbmzuy.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://3g.fanxiaobao.xyz/Article/details/glqaxyohq.sHtML

[Q74] 强制使用索引
来源：http://mobile.fanxiaobao.xyz/Article/details/gvvqmqfxz.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://blog.fanxiaobao.xyz/Article/details/guewydcsw.sHtML

[Q75] 日期格式化
来源：http://m.share.fanxiaobao.xyz/Article/details/gfmysvjnk.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://blog.fanxiaobao.xyz/Article/details/grziyjqqr.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.share.fanxiaobao.xyz/Article/details/ghrcvkasc.sHtML

[Q76] 按天统计
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geejnfkyu.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://read.share.fanxiaobao.xyz/Article/details/gfhhzgntu.sHtML

[Q77] 时间加减
来源：http://3g.fanxiaobao.xyz/Article/details/gfoxhvswc.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glwahqmhx.sHtML

[Q78] 当前时间
来源：http://baike.fanxiaobao.xyz/Article/details/gjrgkchaq.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://read.share.fanxiaobao.xyz/Article/details/gzwvoxmxk.sHtML

[Q79] 字符串拼接
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqnxlzcnf.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.share.fanxiaobao.xyz/Article/details/gllacogbl.sHtML

[Q80] 字符串截取
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghpdefwjd.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gjmvbvohh.sHtML

[Q81] 字符串替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gipggduoi.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gteworlqr.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.fanxiaobao.xyz/Article/details/gzrhtgfov.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gcmgcikuo.sHtML

[Q83] 大小写转换
来源：http://read.share.fanxiaobao.xyz/Article/details/gqcxzlxch.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gzjhkqcjk.sHtML

[Q84] 去除首尾空格
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvfaucsmb.sHtML

SELECT TRIM(name) FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gyjnuselc.sHtML

[Q85] 数值取整
来源：http://baike.fanxiaobao.xyz/Article/details/gwvdxcoow.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giewmubbk.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtlgdnjvo.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.fanxiaobao.xyz/Article/details/gkbgedulb.sHtML

[Q87] JSON 字段做条件
来源：http://3g.fanxiaobao.xyz/Article/details/goiigimvv.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.fanxiaobao.xyz/Article/details/gjwfuckuk.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkgecbian.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.fanxiaobao.xyz/Article/details/gqdvuaubc.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gcxhtuktf.sHtML

[Q89] 判断表是否存在
来源：http://read.share.fanxiaobao.xyz/Article/details/gjndryfca.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.fanxiaobao.xyz/Article/details/gxfrvpkhm.sHtML

[Q90] 生成序号列
来源：http://baike.fanxiaobao.xyz/Article/details/gzcdopbbq.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://baike.fanxiaobao.xyz/Article/details/ghxzgduro.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/givxeigqq.sHtML

R. Bash 专题
来源：http://m.share.fanxiaobao.xyz/Article/details/gxmkkneri.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gpvcbztsx.sHtML

[R01] shebang 与严格模式
来源：http://wap.fanxiaobao.xyz/Article/details/gkdxskrvh.sHtML

#!/usr/bin/env bash
来源：http://wap.fanxiaobao.xyz/Article/details/geejzghpn.sHtML

set -euo pipefail
来源：http://baike.fanxiaobao.xyz/Article/details/gkfritosh.sHtML

[R02] 变量赋值与使用
来源：http://baike.fanxiaobao.xyz/Article/details/gdihklwmc.sHtML

name="Tom"; echo "$name"
来源：http://baike.fanxiaobao.xyz/Article/details/gzumgrtay.sHtML

[R03] 只读变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gtqfjtxth.sHtML

readonly PI=3.14
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghsxxbttu.sHtML

[R04] 位置参数
来源：http://mobile.fanxiaobao.xyz/Article/details/gbgfcrnxj.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grvrtofiy.sHtML

[R05] 参数默认值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwplndrfp.sHtML

name="${1:-default}"
来源：http://m.share.fanxiaobao.xyz/Article/details/grntkwmma.sHtML

[R06] 判断命令是否存在
来源：http://3g.fanxiaobao.xyz/Article/details/gkguccufr.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gawvqjcwf.sHtML

[R07] if 判断文件
来源：http://3g.fanxiaobao.xyz/Article/details/gehjebtez.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.fanxiaobao.xyz/Article/details/gxcjnsopl.sHtML

[R08] 数值比较
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gppxukvub.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.fanxiaobao.xyz/Article/details/gnajlqqkm.sHtML

[R09] 字符串比较
来源：http://mobile.fanxiaobao.xyz/Article/details/gdusbvgaw.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.fanxiaobao.xyz/Article/details/gkuqkpgeq.sHtML

[R10] 正则匹配
来源：http://blog.fanxiaobao.xyz/Article/details/gqckydtco.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbyqzpgwt.sHtML

[R11] case 多分支
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtiynzkwe.sHtML

case "$1" in
来源：http://read.share.fanxiaobao.xyz/Article/details/gtgskqlzj.sHtML

start) echo "启动" ;;
来源：http://read.share.fanxiaobao.xyz/Article/details/giijkwxlp.sHtML

stop)  echo "停止" ;;
来源：http://m.share.fanxiaobao.xyz/Article/details/gwaunxcuh.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.fanxiaobao.xyz/Article/details/gcayrcayk.sHtML

esac
来源：http://www.share.fanxiaobao.xyz/Article/details/gdusqapct.sHtML

[R12] for 遍历文件
来源：http://3g.fanxiaobao.xyz/Article/details/gwedhtgey.sHtML

for f in *.txt; do echo "$f"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gftsnutpx.sHtML

[R13] for 计数循环
来源：http://m.share.fanxiaobao.xyz/Article/details/gqanskiuo.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gwdgspafo.sHtML

[R14] C 风格 for
来源：http://blog.fanxiaobao.xyz/Article/details/gmwrxnzso.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gfoumhxpa.sHtML

[R15] while 逐行读文件
来源：http://wap.fanxiaobao.xyz/Article/details/gobrdbaoz.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gspkfwotj.sHtML

[R16] until 等待条件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsmuyeqip.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gbanyrppw.sHtML

[R17] 数组定义与取值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcvxnpjuc.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.fanxiaobao.xyz/Article/details/gweykbwip.sHtML

[R18] 遍历数组
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnwtagcuq.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.fanxiaobao.xyz/Article/details/gwrnypezv.sHtML

[R19] 数组长度
来源：http://wap.fanxiaobao.xyz/Article/details/grkmecuwh.sHtML

echo "${#arr[@]}"
来源：http://blog.fanxiaobao.xyz/Article/details/geucodqgk.sHtML

[R20] 关联数组（字典）
来源：http://www.share.fanxiaobao.xyz/Article/details/guwikjkur.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.fanxiaobao.xyz/Article/details/gdfgoscnl.sHtML

[R21] 字符串长度
来源：http://baike.fanxiaobao.xyz/Article/details/glcirqxhn.sHtML

echo "${#s}"
来源：http://baike.fanxiaobao.xyz/Article/details/glgclmlmb.sHtML

[R22] 截取子串
来源：http://mobile.fanxiaobao.xyz/Article/details/godloyvkv.sHtML

echo "${s:0:5}"
来源：http://3g.fanxiaobao.xyz/Article/details/gozsburjk.sHtML

[R23] 字符串替换
来源：http://blog.fanxiaobao.xyz/Article/details/gkcwxvwph.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.fanxiaobao.xyz/Article/details/gctchxwtl.sHtML

[R24] 大小写转换
来源：http://www.share.fanxiaobao.xyz/Article/details/gedivcpmz.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.fanxiaobao.xyz/Article/details/grpgctbzl.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.fanxiaobao.xyz/Article/details/gwjnqpqvg.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.fanxiaobao.xyz/Article/details/gvgqxpzuc.sHtML

[R26] 命令替换
来源：http://www.share.fanxiaobao.xyz/Article/details/gqahkhzyg.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.fanxiaobao.xyz/Article/details/gpiwdsohe.sHtML

[R27] 算术展开
来源：http://www.share.fanxiaobao.xyz/Article/details/gtboqiypa.sHtML

echo $((1 + 2 * 3))
来源：http://blog.fanxiaobao.xyz/Article/details/guxvkbufl.sHtML

[R28] 浮点运算
来源：http://m.share.fanxiaobao.xyz/Article/details/gyfpjwhmz.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpbswilnm.sHtML

[R29] 定义函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gzasmgjvg.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.fanxiaobao.xyz/Article/details/gnzkocosi.sHtML

[R30] 函数返回状态码
来源：http://3g.fanxiaobao.xyz/Article/details/gcigylxsv.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.fanxiaobao.xyz/Article/details/gpltzulji.sHtML

[R31] 局部变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gadwicrab.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gzbgvvyng.sHtML

[R32] 参数个数校验
来源：http://3g.fanxiaobao.xyz/Article/details/ghwiezjsk.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbqmnejlu.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyiedsuuc.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsagjiggr.sHtML

[R34] 退出时清理
来源：http://mobile.fanxiaobao.xyz/Article/details/ghzybjkht.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fanxiaobao.xyz/Article/details/gnjhmuzrm.sHtML

[R35] 后台执行并等待
来源：http://wap.fanxiaobao.xyz/Article/details/gejdtbprm.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.fanxiaobao.xyz/Article/details/gmoozzxxd.sHtML

[R36] 并发执行多个任务
来源：http://baike.fanxiaobao.xyz/Article/details/glwxhjgan.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.fanxiaobao.xyz/Article/details/gpzuwwxpa.sHtML

[R37] 把输出赋给变量
来源：http://baike.fanxiaobao.xyz/Article/details/gcajaddwb.sHtML

files=$(ls -1)
来源：http://www.share.fanxiaobao.xyz/Article/details/gqxzsccjh.sHtML

[R38] 管道串联
来源：http://baike.fanxiaobao.xyz/Article/details/gweyxftyl.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.fanxiaobao.xyz/Article/details/gbbssoray.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.fanxiaobao.xyz/Article/details/guhfqwnzj.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giktwjsjm.sHtML

[R40] 追加写日志
来源：http://baike.fanxiaobao.xyz/Article/details/gjvpixatb.sHtML

echo "log" >> out.log
来源：http://wap.fanxiaobao.xyz/Article/details/gncykrezj.sHtML

[R41] 丢弃输出
来源：http://read.share.fanxiaobao.xyz/Article/details/guhhqfell.sHtML

cmd >/dev/null 2>&1
来源：http://mobile.fanxiaobao.xyz/Article/details/gcciwhajm.sHtML

[R42] 输入重定向
来源：http://www.share.fanxiaobao.xyz/Article/details/gaffwjowl.sHtML

wc -l < a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gasxwnpwz.sHtML

[R43] 按名字查找文件
来源：http://wap.fanxiaobao.xyz/Article/details/ghkehbuii.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goqhuzrmh.sHtML

[R44] 按修改时间查找
来源：http://www.blog.fanxiaobao.xyz/Article/details/gliahbext.sHtML

find . -mtime -7 -type f
来源：http://blog.fanxiaobao.xyz/Article/details/gjogddqnd.sHtML

[R45] 批量删除
来源：http://wap.fanxiaobao.xyz/Article/details/gohigqopt.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goisbjvyf.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.fanxiaobao.xyz/Article/details/gebokwyoe.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.fanxiaobao.xyz/Article/details/gqzbcwvaj.sHtML

[R47] sed 单行替换
来源：http://blog.fanxiaobao.xyz/Article/details/gdngcgfdr.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gzrezgwkr.sHtML

[R48] awk 取指定列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkxbniexw.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gkbowsxdr.sHtML

[R49] awk 带条件
来源：http://www.share.fanxiaobao.xyz/Article/details/gmkebebwx.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.fanxiaobao.xyz/Article/details/gvrkfphup.sHtML

[R50] awk 求和
来源：http://read.share.fanxiaobao.xyz/Article/details/gsrcykkjs.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwxjhkqpx.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glehaleoz.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.fanxiaobao.xyz/Article/details/gfissmvvn.sHtML

[R52] 统计行数
来源：http://m.share.fanxiaobao.xyz/Article/details/ghnygiqvd.sHtML

wc -l a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtvgfnwjm.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.fanxiaobao.xyz/Article/details/ghjisnfeh.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjiogbesu.sHtML

[R54] 比较两个文件
来源：http://3g.fanxiaobao.xyz/Article/details/glvyfiupa.sHtML

diff a.txt b.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gqkbrugxc.sHtML

[R55] 压缩与解压
来源：http://3g.fanxiaobao.xyz/Article/details/grtczjwyy.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.fanxiaobao.xyz/Article/details/gierkbbta.sHtML

[R56] 远程拷贝
来源：http://3g.fanxiaobao.xyz/Article/details/gicjxirtq.sHtML

scp file user@host:/path/
来源：http://baike.fanxiaobao.xyz/Article/details/glnxxmmuu.sHtML

[R57] 远程执行命令
来源：http://3g.fanxiaobao.xyz/Article/details/gppjireuq.sHtML

ssh user@host 'uptime'
来源：http://baike.fanxiaobao.xyz/Article/details/gtndyeoto.sHtML

[R58] 下载文件
来源：http://baike.fanxiaobao.xyz/Article/details/gvrsxjwas.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.fanxiaobao.xyz/Article/details/gjvaahfxv.sHtML

[R59] 发 POST JSON
来源：http://m.share.fanxiaobao.xyz/Article/details/gznolflul.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzewudtan.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.fanxiaobao.xyz/Article/details/glaowtewg.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.fanxiaobao.xyz/Article/details/gbcopicyw.sHtML

[R61] 磁盘占用
来源：http://www.share.fanxiaobao.xyz/Article/details/gjojqylfw.sHtML

df -h;  du -sh *
来源：http://m.share.fanxiaobao.xyz/Article/details/gafvbigtg.sHtML

[R62] 找最占空间的文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gteymuxlv.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.fanxiaobao.xyz/Article/details/gpstpdrqo.sHtML

[R63] 内存与进程
来源：http://www.share.fanxiaobao.xyz/Article/details/gbqyrasjr.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtoghyssu.sHtML

[R64] 结束进程
来源：http://mobile.fanxiaobao.xyz/Article/details/gcwqegmdy.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.fanxiaobao.xyz/Article/details/gowfnzqzu.sHtML

[R65] 查看端口占用
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzibnyghf.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.fanxiaobao.xyz/Article/details/grzdfkvnw.sHtML

[R66] 定时任务
来源：http://3g.fanxiaobao.xyz/Article/details/grqqwpeso.sHtML

crontab -e;  crontab -l
来源：http://www.share.fanxiaobao.xyz/Article/details/glhllwsgh.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.fanxiaobao.xyz/Article/details/grznuzfbp.sHtML

openssl rand -hex 16
来源：http://m.share.fanxiaobao.xyz/Article/details/ggcmdddpg.sHtML

[R68] 计算文件校验值
来源：http://baike.fanxiaobao.xyz/Article/details/gonqaifsj.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gdqnhwfkx.sHtML

[R69] 生成随机密码
来源：http://3g.fanxiaobao.xyz/Article/details/gpunarzgi.sHtML

head -c 16 /dev/urandom | base64
来源：http://read.share.fanxiaobao.xyz/Article/details/gyplgktfz.sHtML

[R70] 时间戳与互转
来源：http://blog.fanxiaobao.xyz/Article/details/ghxkezwlj.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.fanxiaobao.xyz/Article/details/growgwgpr.sHtML

[R71] 日期格式化
来源：http://baike.fanxiaobao.xyz/Article/details/gzlcfalfk.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsfnfbrol.sHtML

[R72] 等待端口就绪
来源：http://3g.fanxiaobao.xyz/Article/details/gozzmtkgd.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gzfgfogwc.sHtML

[R73] 分割大日志
来源：http://baike.fanxiaobao.xyz/Article/details/gtdfnrwje.sHtML

split -l 1000 big.log part_
来源：http://www.share.fanxiaobao.xyz/Article/details/godgoipbs.sHtML

[R74] 批量重命名
来源：http://www.blog.fanxiaobao.xyz/Article/details/gywubjmuo.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.fanxiaobao.xyz/Article/details/gwwogsyzu.sHtML

[R75] 导出环境变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghecothmq.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.fanxiaobao.xyz/Article/details/ghtauohcg.sHtML

[R76] 使用临时文件
来源：http://baike.fanxiaobao.xyz/Article/details/gcdezfcfq.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.fanxiaobao.xyz/Article/details/guozviqhp.sHtML

[R77] 读取用户输入
来源：http://3g.fanxiaobao.xyz/Article/details/ghvkbmdtt.sHtML

read -rp "请输入: " ans
来源：http://mobile.fanxiaobao.xyz/Article/details/gedgdponb.sHtML

[R78] 交互式菜单
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxwuqzqqu.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.fanxiaobao.xyz/Article/details/ginnzyhpi.sHtML

[R79] 解析命令行选项
来源：http://m.share.fanxiaobao.xyz/Article/details/gymvrqerw.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.fanxiaobao.xyz/Article/details/gsagwztqx.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.fanxiaobao.xyz/Article/details/gjfkhoqxl.sHtML

time ./run.sh
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvfnnzkwg.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gseddliie.sHtML

S. C / C++ 专题
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjmfdbfum.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gqqimqtpr.sHtML

[S01] C：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gflrouyxf.sHtML

#include <stdio.h>
来源：http://m.share.fanxiaobao.xyz/Article/details/gahlfdxce.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.fanxiaobao.xyz/Article/details/gngtlaxfy.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.fanxiaobao.xyz/Article/details/gctmrwwgl.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.fanxiaobao.xyz/Article/details/guapycyfm.sHtML

[S03] C：读入整数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gieflzuhw.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gssmxjywq.sHtML

[S04] C：字符串复制
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwcgwvdld.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.fanxiaobao.xyz/Article/details/ghxzqbtbj.sHtML

[S05] C：字符串长度
来源：http://baike.fanxiaobao.xyz/Article/details/gmztfndbd.sHtML

strlen(s)
来源：http://blog.fanxiaobao.xyz/Article/details/gqmynenry.sHtML

[S06] C：字符串比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxuvefjss.sHtML

strcmp(a, b) == 0
来源：http://mobile.fanxiaobao.xyz/Article/details/gngaecone.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfsneymwf.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.fanxiaobao.xyz/Article/details/grpioipne.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.fanxiaobao.xyz/Article/details/gkovcxbvh.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.fanxiaobao.xyz/Article/details/gisgbtjzy.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.fanxiaobao.xyz/Article/details/gderuptkm.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.fanxiaobao.xyz/Article/details/gukkmmzvb.sHtML

[S10] C：指针与解引用
来源：http://mobile.fanxiaobao.xyz/Article/details/goyfombdr.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.fanxiaobao.xyz/Article/details/ghywbdohv.sHtML

[S11] C：逐行读文件
来源：http://blog.fanxiaobao.xyz/Article/details/gcbxrjozv.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.fanxiaobao.xyz/Article/details/gqqpinxxs.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.fanxiaobao.xyz/Article/details/grihrfbnx.sHtML

fclose(f);
来源：http://baike.fanxiaobao.xyz/Article/details/gltakalak.sHtML

[S12] C：写文件
来源：http://www.share.fanxiaobao.xyz/Article/details/glifygzdu.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.fanxiaobao.xyz/Article/details/gfvmzukrj.sHtML

[S13] C：宏定义
来源：http://baike.fanxiaobao.xyz/Article/details/gxebhcdkt.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guyswakcx.sHtML

[S14] C：枚举
来源：http://read.share.fanxiaobao.xyz/Article/details/ghhqhqgbs.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.fanxiaobao.xyz/Article/details/gbqqlmjcj.sHtML

[S15] C：类型转换
来源：http://mobile.fanxiaobao.xyz/Article/details/gsnlvinxu.sHtML

(double) a / b
来源：http://www.blog.fanxiaobao.xyz/Article/details/gucduwuwx.sHtML

[S16] C：位操作置位
来源：http://wap.fanxiaobao.xyz/Article/details/gkovpufur.sHtML

x |= (1 << 3);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpbxmjzws.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.fanxiaobao.xyz/Article/details/grrgdgjih.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.fanxiaobao.xyz/Article/details/gfptgfaee.sHtML

[S18] C：命令行参数
来源：http://m.share.fanxiaobao.xyz/Article/details/gaadtjtyo.sHtML

int main(int argc, char **argv)
来源：http://wap.fanxiaobao.xyz/Article/details/gfuvieqsc.sHtML

[S19] C：快速排序
来源：http://mobile.fanxiaobao.xyz/Article/details/gaeyqwqoz.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxxmeoewu.sHtML

[S20] C：二分查找
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvuwplmja.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.fanxiaobao.xyz/Article/details/guvnmiotp.sHtML

[S21] C：字符类别判断
来源：http://baike.fanxiaobao.xyz/Article/details/gmfhbzgsc.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.fanxiaobao.xyz/Article/details/groqhaqdv.sHtML

[S22] C：字符串转数字
来源：http://blog.fanxiaobao.xyz/Article/details/gfnopeicq.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.fanxiaobao.xyz/Article/details/gxvtbyipj.sHtML

[S23] C：随机数
来源：http://blog.fanxiaobao.xyz/Article/details/glegvvpqt.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.fanxiaobao.xyz/Article/details/gjeeikgqc.sHtML

[S24] C：获取本地时间
来源：http://read.share.fanxiaobao.xyz/Article/details/ghsyjtkzf.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfuwsmgca.sHtML

[S25] C：内存拷贝
来源：http://wap.fanxiaobao.xyz/Article/details/gofzokyty.sHtML

memcpy(dst, src, n);
来源：http://mobile.fanxiaobao.xyz/Article/details/gtqaclipi.sHtML

[S26] C：内存清零
来源：http://www.share.fanxiaobao.xyz/Article/details/gjfqedidx.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbnzxquiv.sHtML

[S27] C：定义常量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwpgiykif.sHtML

const double PI = 3.14159;
来源：http://3g.fanxiaobao.xyz/Article/details/giagzqgtp.sHtML

[S28] C：静态变量
来源：http://blog.fanxiaobao.xyz/Article/details/gtbvkrfuv.sHtML

static int counter = 0;
来源：http://mobile.fanxiaobao.xyz/Article/details/gqnsvumxx.sHtML

[S29] C：变参函数
来源：http://blog.fanxiaobao.xyz/Article/details/gkotoybpd.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.fanxiaobao.xyz/Article/details/ggodloytj.sHtML

[S30] C：头文件保护
来源：http://3g.fanxiaobao.xyz/Article/details/gggyyyxcm.sHtML

#ifndef X_H
来源：http://3g.fanxiaobao.xyz/Article/details/ghtptqkly.sHtML

#define X_H
来源：http://blog.fanxiaobao.xyz/Article/details/gwljfxjsp.sHtML

#endif
来源：http://baike.fanxiaobao.xyz/Article/details/gujhysczs.sHtML

[S31] C++：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gbgdrxjax.sHtML

#include <iostream>
来源：http://wap.fanxiaobao.xyz/Article/details/gkethfyti.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.fanxiaobao.xyz/Article/details/gvkeoqnrb.sHtML

[S32] C++：字符串
来源：http://baike.fanxiaobao.xyz/Article/details/glnngjnas.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.fanxiaobao.xyz/Article/details/gdajuyflp.sHtML

[S33] C++：vector 增删
来源：http://read.share.fanxiaobao.xyz/Article/details/geuqchdou.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwvshyebe.sHtML

[S34] C++：遍历 vector
来源：http://mobile.fanxiaobao.xyz/Article/details/gqbvgcpfn.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.fanxiaobao.xyz/Article/details/gmrskaole.sHtML


<!-- 参考信息 -->