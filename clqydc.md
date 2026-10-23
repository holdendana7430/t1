代发 wailian999

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3emqlhhqo.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3cmdqmpjp.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3eljbqlix.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3rgthwjdl.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3jfbzyfve.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3puikjean.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3urucgytz.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3nkiuoxye.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3cuglrixf.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3sqismgxm.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3exhayelg.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3xgaaagpx.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3bgqcmxhk.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3bwaprflh.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3cngkxpam.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3obemzefh.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3scsjaaic.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3khglglwr.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3odkmyxfa.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3blngfnnr.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3ivudkyav.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3flmpxhkq.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3dumqxxgy.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3qmqyujmk.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3osqhuivh.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3ohpvtckn.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3nowhtnwq.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3tjxcnpoe.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3fuxccfvg.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3abjwryov.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3zinvlgev.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3zwaxvwce.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3rggcmsal.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3kwajnaxl.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3eradzyvz.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3eldmustq.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3qynezwml.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3lckfhjzf.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3gzarigmt.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3xwwedqnz.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3qgncuuds.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3rqgljlyk.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3kqsnzcol.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3eankngld.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3dunkaccx.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3msyyazjb.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3dofcbwtt.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3tlsszuqv.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3wglxxjdc.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3tefilaqz.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3oinairqf.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3uincrgmz.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3xzgngrok.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3iobkkfda.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3dqomneum.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bamalsho.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3ariicdbo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pmqwebop.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3gtjleuma.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3csswzuop.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3zkjhzyit.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3tfjjqjjz.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3nutmatza.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3gvdhttmj.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3jxzpdykk.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3cwhqbgul.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3enhcrpdy.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3meniepdz.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3qgytrjbz.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3shwvhpur.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3avgrmhts.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3ptrdptnw.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3rzidllyf.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3mmimpcqj.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3kdtxnopm.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3cquhggbc.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3dkpkvuoy.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3ojpcgkcy.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3dnwvtcov.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3ofdfpvzx.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3smluvfsj.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3zhlnhjsq.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3dfjpxxuy.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3bfjyvrau.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3bjrsutcd.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3lajomuor.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3ffrowylr.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3tidvilud.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3gzdcnlsv.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3qjdwhwki.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3tpvpljkr.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3gfchaeku.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3ltjvicbp.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3iokcnelq.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3arteaxzn.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3mbkzceyv.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3vdmxgdez.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3wogqabrs.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3dfafjsar.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3snhcgwla.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3hfjkrqlu.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3glcfjgbn.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3stjmpjkn.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3vdrklpix.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3nvvyjbrh.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3rmmhzaqo.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3gcvqhomt.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3ewhhdpnx.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3rwhzziir.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3epizxtoz.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3lyeuimum.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3zrvzqljn.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3yexztfcf.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3eqgyxocj.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3qpzhadud.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3nnprrust.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3zjzbhyaz.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3zppvgvut.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3mldltxfb.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3sojfxplu.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3bxfxtjya.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3zkbfsqan.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3oltjjzgp.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3rrhooxqy.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3hktepsdv.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3uhushlkd.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3bqlfmmra.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3jbribfmx.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3alodfsrn.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3jqdhzyoz.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3ruduzlzs.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3bpfqbfxg.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3vhoogipz.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3zfykzjqy.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3wcmueknk.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3zziwbode.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3bomnowav.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3ustqojga.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3fsarpynv.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3yzlbbckq.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3pxidnnwy.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3gwxslxqx.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3novlssnf.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3jeezxuse.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3ucrjfoks.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3ecfzmwcv.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3fosvmdcs.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3hpkfupsq.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3jtiojdui.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3vaafnuzo.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3yzkhobsw.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3kzanosny.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3fqueejir.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3ktnpqack.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3zbtqajxp.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3skwhylry.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3sejgkpah.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3abcecswc.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ejuvdxpg.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3penuhabe.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3svyulvgy.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3qydrjgep.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3fntlinox.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3ssrdicvu.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3rrdckttv.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3wrmfgjrl.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3tmgpoazr.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3eivhfwmy.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3zlvjejjp.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3veguvvmk.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3orwwdsru.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3qpnkhtpe.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3qpdffojv.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3guaangty.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3odcenrqx.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3tfsaneuc.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3rrfawnqb.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3vtkbxpex.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3arpxjpfn.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3llgbqhvc.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3naxojegr.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3kdpehhbc.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3saknfgtn.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3idwtffyu.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3mlufqhir.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3mwxezfgr.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3wvkyrhkx.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3apglxecq.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3tpuvhwfp.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3vzuqnmyc.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3mdoryeiv.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3nxjaypyx.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3bcfuchfz.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3corfwkbz.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3pmhrzxyx.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3vlvfxowf.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3stbzqwbv.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3wapyvyuj.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3zwlbogyf.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3hlnkmsvi.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3eefngzxs.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3qraphixw.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3xpnyxenz.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3ybzigmik.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3urwtawiy.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3kncnfcdt.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3ekcenlwy.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3skncprzc.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3kxqeexfx.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3cehynqqc.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3zbeokmyd.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3bbhcggxl.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3dcxrtjjh.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3uujrtple.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3qsokkrcq.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3ggvklgqj.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3afzuewny.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3nfoonirh.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3olrdsmhb.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3cdcbnxok.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3uvjeslzb.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3xfqftyzx.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3pmaybhzj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pmbmkobd.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3qwksklwj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lyouzqna.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3xxbfrqmn.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3ihvgasqo.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3uazmfdyi.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3qywablzf.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3puzmeiwf.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3dugphsvt.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3fchwjnsq.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3veqwkbsa.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3qgpevjbv.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3lnbpxnng.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3yvqpsacv.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3xpuewnga.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3rerwghif.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3yqpnkyzt.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3joglreez.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3cbimeyfx.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3sknylouw.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3sqckzlpn.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3ggbjgcum.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3urilehwg.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3rfqxumwn.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3rveidlsv.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3cpilvaff.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3bprhfdtb.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3azabtmxk.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3dvmqvswg.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3kymueofr.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3tqqaubap.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3nlpaodex.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3xtjesfvp.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3vwqykydj.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3hnmlaipj.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3kjobyokn.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3yiwrkxhk.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3vxpzsezf.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3dsadhudk.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3tbbblldz.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3ipojhcvw.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3xkfgrild.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3xvjlotda.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3wfzjrmij.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3jhdlxupg.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3bebtjpob.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3cyqezygv.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3dnsfawev.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3nseousfe.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3bstvotwy.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3tjwbagkh.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3fskpknqq.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3dgfizniq.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3ounesmhx.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3grswbnxi.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3njpqcvqc.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3gfuudzoo.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3swuvkyaa.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3nwkuqsan.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3yboyhqtb.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3dcsiinbq.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3fsrvikes.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3eiwpbuqb.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3smmlvajb.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3fkeassmm.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3qjrekqxx.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3vdhyoorn.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3pgryozbh.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3sjrnxlds.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3sbbjxmrp.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3tedqytsk.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3chdcomxx.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3wozrhafb.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3lskdzfgg.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3eglzikiu.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3ravxsrtg.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3qsuyffzc.html


<!-- 参考信息 -->