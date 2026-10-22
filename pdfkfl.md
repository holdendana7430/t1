代发 wailian999

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2yzrhpjgc.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2kaaaawok.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2vbntjzra.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2lxnoshoh.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2eaqbjpoq.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2ppyytbbx.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2iylaarta.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2qrxlzoup.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2nmherbwn.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2rnzwkbui.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2bthirsuw.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2gthbhbjt.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2ffhltsih.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2zqtmglmw.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2qkuhnbey.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2bcmszkef.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2whfsmcya.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2gyjcxbuy.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2hrsuobed.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2slqoqnru.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2lsetbsce.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2uapbdrdn.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2mstpvbph.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2ljuqqopd.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2unfevpfb.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2sqixcyvw.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2wjhbjsfr.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2dygyzhyf.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2kfjjzbor.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2yfffbzcz.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2tmzhfzty.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2qhyubwbr.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2qeirroru.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2yobsnshy.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2kumfdnjn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mcpehibm.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2vmqlewcr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rszqebie.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2kkdyqzdj.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2egvhangk.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2renrlhox.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2bgzfyjuc.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2oyzujvbf.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2fkrklobb.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2urjxcijv.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2ndwihxlb.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2pdbyvwap.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2totnnodm.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2befounlx.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2anjoqlgp.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2vemrazag.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2fkpcitbg.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2wjmjeckj.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2hekmrtpj.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2ecfjeucy.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2uildfwod.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2pekgitex.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2kknqoapp.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2mwapfdmb.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2iupurcez.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2kaowdhhd.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2wvskcbps.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2ryxiaflo.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2jhyhlztu.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2qkyzuvhe.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2yyctlvhu.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2auhqipdg.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2qpbdcjer.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2ditjeetg.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2ovmoqfzm.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2dqhwnofx.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2cmpjvkrn.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2djesskrr.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2yrlkksii.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2uoeglqra.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2usnpadyv.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2izrgiixb.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2epppfjua.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2lbftclru.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2hvclauep.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2pzsrxuvz.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2fmskobmk.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2ukubilvx.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2febtlmmk.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2uxdoemjh.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2jqsosjuo.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2ypqqlwwn.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2xqyhuyyw.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2pucjoeei.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2fncqaavx.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2unqurchl.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2iqjzxhnu.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2karjoges.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2efadyqwx.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2ejvsgvhc.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2vgpxxhfm.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2jxxlxfyl.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2jsyaqccw.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2cmwwicvd.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2vjebmztb.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2dncbqrgj.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2gbfmhwns.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2tfmzheqp.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2qkfwwzhs.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2cqjknsnk.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2reyuppsj.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2iqevqvma.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2yuzgaucw.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2xnbsustg.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2wzxmufky.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2xvwyjuom.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2ygustvfi.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2vpdbfwyr.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2aligdpwh.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2lulkddvt.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2cjjpnwez.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2yuwdggij.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2qvabcnwb.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2qrdrmoki.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2omfgmdjc.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2ngtksqoa.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2tpzugagu.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2tcufemlh.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2wtjvettl.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2skhoclau.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2lfjjxltg.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2tpiudntv.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2sfjfmdik.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2zyuycsjh.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2ogdrahye.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2dniftuih.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2sjomsivq.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2mymetfea.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2hrvgygll.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2cgzihtga.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2rnhvkzho.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2ncqmsyhz.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2kdldypfi.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2zeojqqzk.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2uvuknism.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2numgfgnr.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2fugxxxkn.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2quqfltal.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2cinuqiqn.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2yzwgpxzb.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2bdpkkeht.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2rjmwzazm.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2ligiyibf.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2ooefvygi.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2qrguzdcz.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ukdveuhb.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2mudhzmtx.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2lcenjegr.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2cjuxayzv.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2jrdvopas.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2yqehvyrq.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2tzoufadv.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2kebkkvzm.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2rqjxkuby.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2kfabxwxp.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2ozjfxuoa.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2zssdsfic.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2nfxgvsto.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2hsukzbvl.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2bvobyfdf.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2gpsezkuy.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2dwchejsm.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2eescgqfq.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2mbkxqhtd.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2kzqzzcmp.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2bggivlfj.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2nllriftq.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2euylyurf.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2twpwjhwt.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2psvbrnbe.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2rpmxpysq.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2icszxval.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2lsbpfqef.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2pndubgdl.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2vhffdjet.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2kczhbgfb.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2wexcesct.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2iropuynr.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2ieafphnl.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2ifbiycfk.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2mmxedqrm.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2abtbhkqb.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2whlyfndd.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2bwrjdahc.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2oewdaxma.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2jxdmgeix.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2yjezabgl.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2vndabrgm.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2geqaiqdf.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2qwaqzevh.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2drvduirz.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2fpibotyu.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2rmhmjhit.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2aiuaqrco.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2qyobcvui.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2zygcaqse.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2njczqcct.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2edtuicll.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kepjhqtl.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2uqqeiaiq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ckwddbpu.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2pagojzqa.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2mjlezghq.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2cnnctvsc.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2lydurezm.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2reilbrbw.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2tvetsyfy.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2luypiydi.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2hujkcfsx.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2qndreeun.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2rtgwxcge.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2dxwdxnxz.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2lwcdfith.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2ugmvbavg.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2gzcfakzh.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2taynxvzp.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2krumqbdr.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2gcxgdocy.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2jgdorzjh.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2ofqkomhh.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2mesarpkb.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2omrwzxyc.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2wjobutdc.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2vwhdzjzh.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2mryhruct.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2lobtkmpq.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2azdxcgqz.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2cbimdfkc.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2koyiyczp.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2lrmkgsho.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2riyoivrh.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2ljhlafrs.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2plikwygy.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2ppdnelri.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2sljmuylb.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2hywpuvrl.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2mkgsxucf.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2tyjgmwyw.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2oqfqlcmk.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2osxfryst.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2ctyylckg.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2tmaqyxrl.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2mzyxwxaz.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2ykmkbmfm.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2kwdnujmt.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2bymlgyfo.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2oqshwgsj.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2ytyyqhsi.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2jjndldgy.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2tagzieao.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2atcruigp.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2ypfcnxbo.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2xguynbbj.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2vbpprfcf.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2uassvqzm.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2jcvfgnrf.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2qndizycg.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2hogwzukt.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2bmofcwkr.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2qodgzuud.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2nszoylro.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2grolkxux.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2tnajyfdg.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2srsnhfpr.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2qepdsbqq.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2rsjmggqt.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2wqpfijmp.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2pycxwqog.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2ijdftbgt.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2gxotwkjj.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2ljnpadrw.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2wosjdllt.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2tcnnqzjd.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2cufusokq.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2unwyaxck.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2bevjuvld.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2bkbtjbnu.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2stwcivyq.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2flglruhx.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2lexatiur.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2nqupdvcv.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2ykbrxrul.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2upbwrhli.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2fnkrzdsz.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2wrllkxhd.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2vjogweem.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2izxugvlv.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2ggttcqeb.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2dlqttgoc.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2npxgrjro.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2nowgjekg.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2tjczzdjo.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2llswunch.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2qeowfntb.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2ewfshsrj.html


<!-- 参考信息 -->