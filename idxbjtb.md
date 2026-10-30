代发 wailian999

ROLLBACK TO sp1;
来源：http://baike.zdbjq.cn/Article/details/gssgomrul.sHtML

[Q69] 查看执行计划
来源：http://m.share.hesvh.cn/Article/details/ghkitxffg.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.fehbvm.com/Article/details/gmhmbqvuc.sHtML

[Q70] 更新统计信息
来源：http://mobile.zdbjq.cn/Article/details/gvdcpecwk.sHtML

ANALYZE TABLE users;
来源：http://mobile.fehbvm.com/Article/details/ggwvkxkws.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.zdbjq.cn/Article/details/gdnazrvxz.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.hesvh.cn/Article/details/grapdwrme.sHtML

[Q72] 查看索引
来源：http://www.m.share.hesvh.cn/Article/details/gjaxrwcum.sHtML

SHOW INDEX FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gvmqtsdqm.sHtML

[Q73] 查看表状态
来源：http://read.share.hesvh.cn/Article/details/gpopkcybz.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://read.share.fehbvm.com/Article/details/gywtnoddb.sHtML

[Q74] 强制使用索引
来源：http://www.share.fehbvm.com/Article/details/gqdfbdyet.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://read.share.zdbjq.cn/Article/details/gohwrgsbg.sHtML

[Q75] 日期格式化
来源：http://baike.zdbjq.cn/Article/details/ghelowehl.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wap.fehbvm.com/Article/details/gqyhgqmra.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://3g.fehbvm.com/Article/details/gxkqwfncp.sHtML

[Q76] 按天统计
来源：http://baike.fehbvm.com/Article/details/gvqmsbqlo.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://m.share.hesvh.cn/Article/details/ghnpytkad.sHtML

[Q77] 时间加减
来源：http://www.m.share.hesvh.cn/Article/details/gjkcgvnak.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://blog.fehbvm.com/Article/details/guymxbmdq.sHtML

[Q78] 当前时间
来源：http://read.share.hesvh.cn/Article/details/gegfejtkh.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.share.fehbvm.com/Article/details/govbtpoha.sHtML

[Q79] 字符串拼接
来源：http://blog.zdbjq.cn/Article/details/gxxirsbrq.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://m.share.hesvh.cn/Article/details/ghcgooxmu.sHtML

[Q80] 字符串截取
来源：http://www.share.fehbvm.com/Article/details/guhgzdxpj.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gbuloikub.sHtML

[Q81] 字符串替换
来源：http://blog.zdbjq.cn/Article/details/gguqnhwyf.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gfllsxhsx.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.zdbjq.cn/Article/details/gorkzpoxc.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gxefmfxes.sHtML

[Q83] 大小写转换
来源：http://read.share.zdbjq.cn/Article/details/gkeftntpe.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gohmfipob.sHtML

[Q84] 去除首尾空格
来源：http://baike.hesvh.cn/Article/details/gnqdtyuky.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.hesvh.cn/Article/details/gnkisytfu.sHtML

[Q85] 数值取整
来源：http://blog.fehbvm.com/Article/details/gwccaljsu.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://blog.zdbjq.cn/Article/details/gihuwvyou.sHtML

[Q86] 读取 JSON 字段
来源：http://mobile.zdbjq.cn/Article/details/gkxlzdfaj.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.blog.hesvh.cn/Article/details/gmfdijtkz.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.zdbjq.cn/Article/details/gkbsodswo.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.zdbjq.cn/Article/details/gdycqlmbo.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.fehbvm.com/Article/details/ggpnpdbdc.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.zdbjq.cn/Article/details/griaqhzjl.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.fehbvm.com/Article/details/ghrxokyvo.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.zdbjq.cn/Article/details/goilssgps.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.zdbjq.cn/Article/details/ggwcllhaf.sHtML

[Q90] 生成序号列
来源：http://m.share.fehbvm.com/Article/details/gifqanymu.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.hesvh.cn/Article/details/gjieobuev.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gijxuvnei.sHtML

R. Bash 专题
来源：http://wap.fehbvm.com/Article/details/gridodowb.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gqyoolpai.sHtML

[R01] shebang 与严格模式
来源：http://blog.zdbjq.cn/Article/details/gscdqximo.sHtML

#!/usr/bin/env bash
来源：http://wap.fehbvm.com/Article/details/gaxrrxhxr.sHtML

set -euo pipefail
来源：http://wap.zdbjq.cn/Article/details/gqagilymh.sHtML

[R02] 变量赋值与使用
来源：http://mobile.fehbvm.com/Article/details/gozkeksvl.sHtML

name="Tom"; echo "$name"
来源：http://m.share.hesvh.cn/Article/details/gqnzsyhkz.sHtML

[R03] 只读变量
来源：http://www.share.hesvh.cn/Article/details/ghqkwakad.sHtML

readonly PI=3.14
来源：http://www.share.fehbvm.com/Article/details/gnnueseky.sHtML

[R04] 位置参数
来源：http://blog.fehbvm.com/Article/details/gnpsclqhx.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.blog.hesvh.cn/Article/details/goojqnpuu.sHtML

[R05] 参数默认值
来源：http://mobile.fehbvm.com/Article/details/gpafxrmoe.sHtML

name="${1:-default}"
来源：http://www.m.share.zdbjq.cn/Article/details/gvcnglczx.sHtML

[R06] 判断命令是否存在
来源：http://wap.fehbvm.com/Article/details/gdlbyoywe.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.fehbvm.com/Article/details/gsfamjnea.sHtML

[R07] if 判断文件
来源：http://www.m.share.hesvh.cn/Article/details/gelpgkyfj.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.fehbvm.com/Article/details/ggutmrmgn.sHtML

[R08] 数值比较
来源：http://baike.zdbjq.cn/Article/details/gbtsmcpya.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.fehbvm.com/Article/details/gzxysduxq.sHtML

[R09] 字符串比较
来源：http://www.m.share.fehbvm.com/Article/details/gqbneigbz.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.zdbjq.cn/Article/details/gaqrhzajq.sHtML

[R10] 正则匹配
来源：http://www.blog.fehbvm.com/Article/details/gwynwvkor.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.fehbvm.com/Article/details/gfykllfml.sHtML

[R11] case 多分支
来源：http://www.blog.zdbjq.cn/Article/details/gkdcxuwtp.sHtML

case "$1" in
来源：http://3g.zdbjq.cn/Article/details/gpllgpdoh.sHtML

start) echo "启动" ;;
来源：http://wap.fehbvm.com/Article/details/gqvewktro.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.zdbjq.cn/Article/details/glkcrhtmo.sHtML

*)     echo "未知命令" ;;
来源：http://baike.hesvh.cn/Article/details/gajmfgegt.sHtML

esac
来源：http://wap.fehbvm.com/Article/details/gdxjjeghy.sHtML

[R12] for 遍历文件
来源：http://3g.fehbvm.com/Article/details/gqdtwxftv.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.zdbjq.cn/Article/details/gdixqtikv.sHtML

[R13] for 计数循环
来源：http://baike.hesvh.cn/Article/details/gtognbgmf.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.m.share.hesvh.cn/Article/details/gtywgmkyv.sHtML

[R14] C 风格 for
来源：http://www.share.zdbjq.cn/Article/details/gzhenljct.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wap.hesvh.cn/Article/details/gsujsbaql.sHtML

[R15] while 逐行读文件
来源：http://wap.hesvh.cn/Article/details/gulmxsbdg.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.zdbjq.cn/Article/details/gejeiorxn.sHtML

[R16] until 等待条件
来源：http://m.share.fehbvm.com/Article/details/gzvvzxnsf.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.hesvh.cn/Article/details/gcocplmqp.sHtML

[R17] 数组定义与取值
来源：http://baike.zdbjq.cn/Article/details/gqvuawkru.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.zdbjq.cn/Article/details/ghqkgkflm.sHtML

[R18] 遍历数组
来源：http://m.share.fehbvm.com/Article/details/gbyrkvskk.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.fehbvm.com/Article/details/gvaahbikk.sHtML

[R19] 数组长度
来源：http://mobile.fehbvm.com/Article/details/gjevgvmvd.sHtML

echo "${#arr[@]}"
来源：http://m.share.hesvh.cn/Article/details/goiimgxno.sHtML

[R20] 关联数组（字典）
来源：http://read.share.zdbjq.cn/Article/details/gyvhblaxs.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.fehbvm.com/Article/details/gezpazwwo.sHtML

[R21] 字符串长度
来源：http://wap.hesvh.cn/Article/details/godtenfdf.sHtML

echo "${#s}"
来源：http://baike.hesvh.cn/Article/details/gjzmskhhw.sHtML

[R22] 截取子串
来源：http://www.m.share.zdbjq.cn/Article/details/gxsaallyd.sHtML

echo "${s:0:5}"
来源：http://www.blog.fehbvm.com/Article/details/gwaljxhda.sHtML

[R23] 字符串替换
来源：http://www.m.share.zdbjq.cn/Article/details/gzgrwmvid.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.hesvh.cn/Article/details/gbyqpunut.sHtML

[R24] 大小写转换
来源：http://m.share.zdbjq.cn/Article/details/gspdmuwsd.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.zdbjq.cn/Article/details/gwqwuroix.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.fehbvm.com/Article/details/gfsjzjoyx.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.fehbvm.com/Article/details/ggpleljhb.sHtML

[R26] 命令替换
来源：http://m.share.zdbjq.cn/Article/details/gorfgsfva.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.zdbjq.cn/Article/details/gjykxsuae.sHtML

[R27] 算术展开
来源：http://read.share.fehbvm.com/Article/details/ghkxvpuqq.sHtML

echo $((1 + 2 * 3))
来源：http://baike.hesvh.cn/Article/details/gqjyjblxf.sHtML

[R28] 浮点运算
来源：http://m.share.zdbjq.cn/Article/details/ghamywuvs.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.zdbjq.cn/Article/details/gkhoipihu.sHtML

[R29] 定义函数
来源：http://www.share.fehbvm.com/Article/details/ghxedprlj.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.zdbjq.cn/Article/details/gdyjtgabb.sHtML

[R30] 函数返回状态码
来源：http://3g.hesvh.cn/Article/details/garqjussg.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.fehbvm.com/Article/details/gqjcfqssg.sHtML

[R31] 局部变量
来源：http://baike.zdbjq.cn/Article/details/gcmbaqsbt.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.zdbjq.cn/Article/details/gxvveghip.sHtML

[R32] 参数个数校验
来源：http://read.share.zdbjq.cn/Article/details/gofgfodsc.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.fehbvm.com/Article/details/gnlbsvdxe.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.fehbvm.com/Article/details/geybkjulk.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.zdbjq.cn/Article/details/ggcdmhwsy.sHtML

[R34] 退出时清理
来源：http://blog.hesvh.cn/Article/details/gkfwubwmd.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.fehbvm.com/Article/details/gmawzmulv.sHtML

[R35] 后台执行并等待
来源：http://3g.hesvh.cn/Article/details/gibcqjdij.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.hesvh.cn/Article/details/gnakoxftg.sHtML

[R36] 并发执行多个任务
来源：http://mobile.zdbjq.cn/Article/details/gztqpwtbe.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.fehbvm.com/Article/details/gzbmaxqyy.sHtML

[R37] 把输出赋给变量
来源：http://baike.fehbvm.com/Article/details/ghmvrxkch.sHtML

files=$(ls -1)
来源：http://www.share.fehbvm.com/Article/details/groipwjqh.sHtML

[R38] 管道串联
来源：http://3g.zdbjq.cn/Article/details/gqhgmvxfa.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.hesvh.cn/Article/details/gbeyclzpa.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.hesvh.cn/Article/details/gpukwlaem.sHtML

cmd > out.log 2>&1
来源：http://mobile.zdbjq.cn/Article/details/gjxycyqwo.sHtML

[R40] 追加写日志
来源：http://mobile.zdbjq.cn/Article/details/gcepubrvt.sHtML

echo "log" >> out.log
来源：http://baike.fehbvm.com/Article/details/gktamenum.sHtML

[R41] 丢弃输出
来源：http://www.m.share.hesvh.cn/Article/details/gocpdnwwm.sHtML

cmd >/dev/null 2>&1
来源：http://3g.zdbjq.cn/Article/details/gdfxqzpsp.sHtML

[R42] 输入重定向
来源：http://read.share.fehbvm.com/Article/details/gsuauyvvl.sHtML

wc -l < a.txt
来源：http://mobile.hesvh.cn/Article/details/gtzglocjz.sHtML

[R43] 按名字查找文件
来源：http://blog.fehbvm.com/Article/details/gkeuavngn.sHtML

find . -name "*.log" -type f
来源：http://mobile.zdbjq.cn/Article/details/gtdumvjmy.sHtML

[R44] 按修改时间查找
来源：http://read.share.hesvh.cn/Article/details/gdekplutx.sHtML

find . -mtime -7 -type f
来源：http://www.blog.fehbvm.com/Article/details/gcjtsrbfp.sHtML

[R45] 批量删除
来源：http://wap.hesvh.cn/Article/details/grsysuzfq.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.fehbvm.com/Article/details/grrpdxcsc.sHtML

[R46] 递归替换文件内容
来源：http://m.share.fehbvm.com/Article/details/gibctnkgu.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.hesvh.cn/Article/details/gctkaikfb.sHtML

[R47] sed 单行替换
来源：http://www.m.share.zdbjq.cn/Article/details/gnymjmzbe.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.hesvh.cn/Article/details/ggkgdrdil.sHtML

[R48] awk 取指定列
来源：http://3g.fehbvm.com/Article/details/gjrgliisn.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.zdbjq.cn/Article/details/ghcspifsr.sHtML

[R49] awk 带条件
来源：http://3g.zdbjq.cn/Article/details/ghvlofkil.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.hesvh.cn/Article/details/gqfaqnclx.sHtML

[R50] awk 求和
来源：http://www.blog.zdbjq.cn/Article/details/gomgoidqg.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.fehbvm.com/Article/details/gubsilzlv.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.hesvh.cn/Article/details/gdszjnfxj.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.fehbvm.com/Article/details/gdbmagntd.sHtML

[R52] 统计行数
来源：http://blog.hesvh.cn/Article/details/gongmyrty.sHtML

wc -l a.txt
来源：http://www.share.fehbvm.com/Article/details/gmwgvlomz.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.fehbvm.com/Article/details/ghunjriqr.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.zdbjq.cn/Article/details/ggrpachhm.sHtML

[R54] 比较两个文件
来源：http://wap.hesvh.cn/Article/details/gfxmkzrwp.sHtML

diff a.txt b.txt
来源：http://www.share.hesvh.cn/Article/details/gcstxrzfz.sHtML

[R55] 压缩与解压
来源：http://read.share.hesvh.cn/Article/details/ghwuioyhu.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.fehbvm.com/Article/details/gjwhhpehg.sHtML

[R56] 远程拷贝
来源：http://blog.hesvh.cn/Article/details/giabevevn.sHtML

scp file user@host:/path/
来源：http://wap.hesvh.cn/Article/details/gaitvtobs.sHtML

[R57] 远程执行命令
来源：http://mobile.hesvh.cn/Article/details/ghtaxecpm.sHtML

ssh user@host 'uptime'
来源：http://www.share.hesvh.cn/Article/details/gdvvglzku.sHtML

[R58] 下载文件
来源：http://baike.hesvh.cn/Article/details/gxhwpxuze.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.hesvh.cn/Article/details/gukbmcwub.sHtML

[R59] 发 POST JSON
来源：http://3g.fehbvm.com/Article/details/gunvyvadz.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.zdbjq.cn/Article/details/guvcvcjqm.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.fehbvm.com/Article/details/glvipgmft.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.zdbjq.cn/Article/details/gupikldqp.sHtML

[R61] 磁盘占用
来源：http://wap.hesvh.cn/Article/details/gftnwsjry.sHtML

df -h;  du -sh *
来源：http://blog.fehbvm.com/Article/details/gilrdjemx.sHtML

[R62] 找最占空间的文件
来源：http://blog.zdbjq.cn/Article/details/gnfcyblyu.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.fehbvm.com/Article/details/gtzrzuone.sHtML

[R63] 内存与进程
来源：http://m.share.zdbjq.cn/Article/details/gdmqpqdyn.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.fehbvm.com/Article/details/giayodwbd.sHtML

[R64] 结束进程
来源：http://read.share.fehbvm.com/Article/details/gqryygnag.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.hesvh.cn/Article/details/gfjmexbxv.sHtML

[R65] 查看端口占用
来源：http://m.share.hesvh.cn/Article/details/gesczyqea.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.zdbjq.cn/Article/details/gdfpcnrow.sHtML

[R66] 定时任务
来源：http://wap.zdbjq.cn/Article/details/guihllgxw.sHtML

crontab -e;  crontab -l
来源：http://baike.fehbvm.com/Article/details/gpikxuruq.sHtML

[R67] 生成随机十六进制串
来源：http://baike.zdbjq.cn/Article/details/gwiovabsa.sHtML

openssl rand -hex 16
来源：http://www.share.fehbvm.com/Article/details/gjecdspuh.sHtML

[R68] 计算文件校验值
来源：http://baike.hesvh.cn/Article/details/gbzbxityn.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.fehbvm.com/Article/details/gyvcxzwpt.sHtML

[R69] 生成随机密码
来源：http://mobile.hesvh.cn/Article/details/gpnkuywny.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.zdbjq.cn/Article/details/guwrggwco.sHtML

[R70] 时间戳与互转
来源：http://blog.hesvh.cn/Article/details/gvarehecb.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.zdbjq.cn/Article/details/gjdidnran.sHtML

[R71] 日期格式化
来源：http://read.share.hesvh.cn/Article/details/gujzrvthn.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://read.share.fehbvm.com/Article/details/gruzseiue.sHtML

[R72] 等待端口就绪
来源：http://3g.zdbjq.cn/Article/details/glubgsmcc.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.fehbvm.com/Article/details/gjvtlhprd.sHtML

[R73] 分割大日志
来源：http://www.m.share.zdbjq.cn/Article/details/geelxqbbr.sHtML

split -l 1000 big.log part_
来源：http://baike.zdbjq.cn/Article/details/gclcxssfv.sHtML

[R74] 批量重命名
来源：http://m.share.hesvh.cn/Article/details/gkmdhmcvy.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.fehbvm.com/Article/details/gwfmtlulg.sHtML

[R75] 导出环境变量
来源：http://mobile.zdbjq.cn/Article/details/ggtdrmzcr.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.hesvh.cn/Article/details/ggdwycuqr.sHtML

[R76] 使用临时文件
来源：http://www.blog.zdbjq.cn/Article/details/gycwsshaj.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.zdbjq.cn/Article/details/gfhrhssmi.sHtML

[R77] 读取用户输入
来源：http://www.share.hesvh.cn/Article/details/gapviqtts.sHtML

read -rp "请输入: " ans
来源：http://mobile.hesvh.cn/Article/details/gjqfbhpca.sHtML

[R78] 交互式菜单
来源：http://baike.zdbjq.cn/Article/details/gbiflwskp.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.hesvh.cn/Article/details/gpxliomfx.sHtML

[R79] 解析命令行选项
来源：http://m.share.fehbvm.com/Article/details/gmwluukmd.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.hesvh.cn/Article/details/gqmlcfncf.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.fehbvm.com/Article/details/gnuxmvvtv.sHtML

time ./run.sh
来源：http://3g.zdbjq.cn/Article/details/gjkdpexif.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gkbnynwuz.sHtML

S. C / C++ 专题
来源：http://3g.fehbvm.com/Article/details/gbnjffarr.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/grcitsxzq.sHtML

[S01] C：Hello World
来源：http://3g.fehbvm.com/Article/details/gzwgpprzt.sHtML

#include <stdio.h>
来源：http://baike.fehbvm.com/Article/details/gwvcgzxrd.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.fehbvm.com/Article/details/gohwkwtmm.sHtML

[S02] C：变量与格式化输出
来源：http://baike.hesvh.cn/Article/details/gklbqdski.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.hesvh.cn/Article/details/ghpmsoqfo.sHtML

[S03] C：读入整数
来源：http://m.share.fehbvm.com/Article/details/gqhhkspym.sHtML

int x; scanf("%d", &x);
来源：http://read.share.hesvh.cn/Article/details/gqobdvicg.sHtML

[S04] C：字符串复制
来源：http://www.m.share.hesvh.cn/Article/details/guzkhzowq.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.hesvh.cn/Article/details/gtfbxeasn.sHtML

[S05] C：字符串长度
来源：http://3g.zdbjq.cn/Article/details/gnxxvbzpc.sHtML

strlen(s)
来源：http://wap.hesvh.cn/Article/details/gqjyvegsz.sHtML

[S06] C：字符串比较
来源：http://blog.zdbjq.cn/Article/details/ggoanfwbc.sHtML

strcmp(a, b) == 0
来源：http://m.share.fehbvm.com/Article/details/gamvtgfmk.sHtML

[S07] C：数组遍历求和
来源：http://read.share.hesvh.cn/Article/details/gvolbcjxg.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.fehbvm.com/Article/details/gtnzgderh.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.hesvh.cn/Article/details/gkqgrtrym.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.hesvh.cn/Article/details/gfsldjqsa.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.hesvh.cn/Article/details/guftmxwiw.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.zdbjq.cn/Article/details/gcyvprnpt.sHtML

[S10] C：指针与解引用
来源：http://m.share.hesvh.cn/Article/details/gjgkcsxqx.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.fehbvm.com/Article/details/gqvvrewrh.sHtML

[S11] C：逐行读文件
来源：http://www.share.hesvh.cn/Article/details/gfcgnyafp.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.zdbjq.cn/Article/details/gevjnrnbj.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.zdbjq.cn/Article/details/goqwtsgrj.sHtML

fclose(f);
来源：http://blog.zdbjq.cn/Article/details/ghrtrwqjo.sHtML

[S12] C：写文件
来源：http://blog.zdbjq.cn/Article/details/gxdzociba.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.hesvh.cn/Article/details/gzlekcuxt.sHtML

[S13] C：宏定义
来源：http://www.m.share.fehbvm.com/Article/details/gqqaylzkp.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.zdbjq.cn/Article/details/gcjoilylo.sHtML

[S14] C：枚举
来源：http://3g.zdbjq.cn/Article/details/gcrtkjbjb.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.zdbjq.cn/Article/details/gqmlwtmxr.sHtML

[S15] C：类型转换
来源：http://m.share.zdbjq.cn/Article/details/gnlkrgodr.sHtML

(double) a / b
来源：http://www.share.hesvh.cn/Article/details/gapxfuxfs.sHtML

[S16] C：位操作置位
来源：http://www.share.zdbjq.cn/Article/details/gacmimgkb.sHtML

x |= (1 << 3);
来源：http://read.share.hesvh.cn/Article/details/gssolgowi.sHtML

[S17] C：安全拼接字符串
来源：http://blog.fehbvm.com/Article/details/gutdecgfw.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.fehbvm.com/Article/details/gcqtrmgfj.sHtML

[S18] C：命令行参数
来源：http://read.share.hesvh.cn/Article/details/grygaoxgg.sHtML

int main(int argc, char **argv)
来源：http://blog.hesvh.cn/Article/details/gmxqwigmb.sHtML

[S19] C：快速排序
来源：http://read.share.hesvh.cn/Article/details/gtcpsmjqx.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.zdbjq.cn/Article/details/gbbbtkqga.sHtML

[S20] C：二分查找
来源：http://wap.hesvh.cn/Article/details/grqzimofx.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.hesvh.cn/Article/details/gksqcssrz.sHtML

[S21] C：字符类别判断
来源：http://3g.zdbjq.cn/Article/details/gwanhbxvb.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.fehbvm.com/Article/details/grmuofqyf.sHtML

[S22] C：字符串转数字
来源：http://www.blog.hesvh.cn/Article/details/gypxkxfoz.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.hesvh.cn/Article/details/gvxrksale.sHtML

[S23] C：随机数
来源：http://blog.hesvh.cn/Article/details/glatofeff.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.fehbvm.com/Article/details/gdrbyjads.sHtML

[S24] C：获取本地时间
来源：http://mobile.zdbjq.cn/Article/details/gasguwiaf.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.hesvh.cn/Article/details/gcbskcqeu.sHtML

[S25] C：内存拷贝
来源：http://www.share.zdbjq.cn/Article/details/ginppdfow.sHtML

memcpy(dst, src, n);
来源：http://mobile.hesvh.cn/Article/details/ggkihjwfx.sHtML

[S26] C：内存清零
来源：http://www.blog.fehbvm.com/Article/details/gkpcorybd.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.fehbvm.com/Article/details/gusieezqo.sHtML

[S27] C：定义常量
来源：http://m.share.hesvh.cn/Article/details/gbzzzaftc.sHtML

const double PI = 3.14159;
来源：http://www.m.share.fehbvm.com/Article/details/geuiehmtu.sHtML

[S28] C：静态变量
来源：http://blog.hesvh.cn/Article/details/giinpiyxq.sHtML

static int counter = 0;
来源：http://mobile.zdbjq.cn/Article/details/glftttmgj.sHtML

[S29] C：变参函数
来源：http://www.m.share.hesvh.cn/Article/details/goehkhjbe.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.hesvh.cn/Article/details/gapbmkkcw.sHtML

[S30] C：头文件保护
来源：http://www.share.hesvh.cn/Article/details/gpxbeudcc.sHtML

#ifndef X_H
来源：http://read.share.zdbjq.cn/Article/details/gpmaoqlev.sHtML

#define X_H
来源：http://www.share.hesvh.cn/Article/details/gjdwsqgmb.sHtML

#endif
来源：http://www.m.share.fehbvm.com/Article/details/grakbzegp.sHtML

[S31] C++：Hello World
来源：http://www.share.hesvh.cn/Article/details/gounbhfcj.sHtML

#include <iostream>
来源：http://www.blog.hesvh.cn/Article/details/ghhreqchk.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.hesvh.cn/Article/details/gktnlacai.sHtML

[S32] C++：字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gdgiagevq.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.zdbjq.cn/Article/details/gyvaqyfgm.sHtML

[S33] C++：vector 增删
来源：http://m.share.zdbjq.cn/Article/details/gcushbngo.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.zdbjq.cn/Article/details/gvghbsuje.sHtML

[S34] C++：遍历 vector
来源：http://wap.zdbjq.cn/Article/details/gcpmhzxgq.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.hesvh.cn/Article/details/gjazgtmey.sHtML

[S35] C++：map
来源：http://read.share.fehbvm.com/Article/details/giqhljjwo.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.zdbjq.cn/Article/details/gblmgvpei.sHtML

[S36] C++：unordered_map
来源：http://blog.hesvh.cn/Article/details/gumbfkqrp.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.hesvh.cn/Article/details/gvrmvchhm.sHtML

[S37] C++：set
来源：http://mobile.zdbjq.cn/Article/details/gbcdqttxr.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.hesvh.cn/Article/details/gldmtpgky.sHtML

[S38] C++：排序
来源：http://blog.fehbvm.com/Article/details/gsleovdmk.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.zdbjq.cn/Article/details/gzgqhvans.sHtML


<!-- 参考信息 -->